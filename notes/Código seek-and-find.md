Aqui escribo los pasos que debo completar en las modificaciones del codigo fuente el cooperation rig para realizar el entrenamiento propuesto, conocido como: Seek-and-find approach.

1. Inter-trial interval: Se aplicará solo cuando haya un caso de exito. Para ello modifico la transición al Estado de "iti" en todos los modos para que solo se active en sus respectivos casos de exito.
	Ejemplo:
	
		self.sm.add_state(name='iti', statetimer= interTrialInterval if previousOutcome > 0 and previousOutcome < 4 else 0 ,
		transitions={'Tup':'readyForNextTrial'},
		outputsOff=[LED1, LED2, Water1, Water2])
2. Cambio de par de puertos: Solo se cambiara el puerto en cada stage si el ultimo trial ha sido exitoso (siendo el significado de exito dependiente del stage).
	Ejemplo: 