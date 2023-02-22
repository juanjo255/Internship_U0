Aqui escribo los pasos que debo completar en las modificaciones del codigo fuente el cooperation rig para realizar el entrenamiento propuesto, conocido como: Seek-and-find approach.

1. **Inter-trial interval:** Se aplicará solo cuando haya un caso de exito. Para ello modifico la transición al Estado de "iti" en todos los modos para que solo se active en sus respectivos casos de exito, ademas se movió al principio del código.
	Ejemplo:
```
	self.sm.add_state(name='iti', statetimer= 
	interTrialInterval if previousOutcome > 0 and previousOutcome < 4 else 0,
	transitions={'Tup':'readyForNextTrial'}, outputsOff=[LED1, LED2, Water1, 
	Water2])
```
2. **Cambio de par de puertos:** Solo se cambiara el puerto en cada stage si el ultimo trial ha sido exitoso (siendo el significado de exito dependiente del stage). Para esto se creo un metodo para la clase "Paradigm" llamada swith_active_side. **Uso limitado de puertos:** A la funcion anterior hay que hacerle un retoque. Se le debe agregar una variable para medir que un puerto no se elija más de n veces seguidas durante el cambio aleatorio.
	Resultado:

```
def switch_active_side(self, previousOutcome, active_side) -> tuple:

	sides= self.params['activeSide'].get_items()
	
	if previousOutcome:
		new_active_side=np.random.choice([0,1])
	if active_side == sides[new_active_side]:
		self.limit_use += 1
		if self.limit_use > self.params['limitPort'].get_value():
			active_side = sides[new_active_side-1]
		else:
			self.limit_use = 0
			active_side=sides[new_active_side]
	if (active_side=='north'):
		port1in = 'S1in'; port2in = 'S2in'
		LED1 = 'S1LED'; LED2 = 'S2LED'
		Water1 = 'S1Water'; Water2 = 'S2Water'
	elif (active_side=='south'):
		port1in = 'N1in'; port2in = 'N2in'
		LED1 = 'N1LED'; LED2 = 'N2LED'
		Water1 = 'N1Water'; Water2 = 'N2Water'
	self.params['activeSide'].set_string(active_side)
	
	return (port1in,port2in,LED1,LED2,Water1,Water2)
```

Finalmente se le tuvo que agregar a cada taskMode la linea de codigo de abajao con el objetivo de almacenar las variables que necesitan los estados de cada taskMode:

```
port1in,port2in,LED1,LED2,Water1,Water2=self.switch_active_side(previousOutcome > 0 and previousOutcome < 4, activeSide)
```

3. 