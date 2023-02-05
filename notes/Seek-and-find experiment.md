#ExperimentDescription

+ This document is a descriptive report of the seek-and-find proposal. It describes all about how could this proposal achieve the purpose of the social cooperation project.
+ If this proposal is approved or taking into account, the idea with the experimental design would be build it from the same template established for the "traditional" approach, but with a few differences.
+ Here I refer to the normal or traditional experiment as the "alternative experiment" and to my proposal as the "randomized experiment" or seek-and-find experiment.


```toc
```



## Philosophy

+ This section describes the reasoning behind the Seek-and-find experiment.

> The state that this approach want to achieve is that, once mice are by their own (lights turned off), they would have to coordinate each other to find the available port, once mice discover the available pair of ports a new pair of port will be selected randomly after n seconds. the need for coordinate their movements in order to find the available pair of ports will make harder to find the available pair of ports the more isolated they are. 


## Objectives

+ This section describes the specifics objectives that need to be follow in order to achieve the general objective of the social cooperation.

### Specific objectives 

> 1. Mice have to be able to use ports.
> 2. Mice have to be able to receive treat using port at the "same time" (during a limited time range once a trial has started).
> 3. Mice have to be able to receive treat using port at the "same time" (during a limited time range once a trial has started) without the help of the experimenter (lights).
> 4. Mice must show a decrease in "performance" reciving treats when they are mutually isolated, that is, when they have lost any kind of "sense" of each other. 

### General objective

> + Identify evidence of social cooperation through the use of the proposed mechanism.

## Key points

+ This section describes the points that makes this proposal different from the alternate experiment.

> 1. **Random use of lights:** This method is used for train the mice in the alternate experiment. During this experiment lights will fulfill the same objective, except that they will indicate the availability of a port not in an alternate behavior but a random behavior (the pair of ports to be open will be random).  
> 2. **Port use limit:** This method will add this new hyperparameter. This hyperparameter will limit the times a port can be use in a row, in such a way we would force the move of the mice. The parameter has to be established over a value of 2, otherwise we would repeating the behavior of the alternate experiment. This port limit will be taught even during the appearance of the light, that is, a pair of light cannot be turned on more than n in a row, where n >= 2.
> 3. **Inter-trial interval:** This is the same hyperparameter as the alternate experiment, but, unlike the aforementioned, in this experiment it will be use in the early stages, in order to give time mice to get away from the port (lose interest) and avoid the lazy behavior.
> 4. **Next port after fail:** The alternate experiment had this parameter established as "alternate", which means that if a mouse activate a trial regardless of if they win or fail (that is they do or not get the reward) the available pair of port changed to the next ones (from north to south and vice versa). In the Seek-and-find experimente this parameter will be established as "fixed", which means that the available pair of port will be choose (randomly) again only if mice win (get the reward).


## Troubleshooting

+ This section describes the problems the Seek-and-find experiment face so far and the solution that this approach gives for each of them. The problems can belong to the alternate experiment or could emerged with the randomized experiment.

> 1. **Go-and-come pattern:** This problem can make the experiment questionable, given that between, for example, for perforate and solid barrier there are barely differences (results with a solid performance of 59% and perforate performance of 59% during same stages), which does not seem to be convincing. Basics statistics say that every mice pair by chance have only 25% of success in every trial (is it really social cooperation?). 
>> **Solution:** Random use of lights.
>>> **Explanation:** Using random use of light we avoid inducing patterns in mice which overshadows social cooperation, if a pattern arised, it would be an independent learnt pattern.
> 2. **The lazy behavior:** This behavior can make questionable our experiment as much as the Go-and-come pattern, it concists of the mice sticking to a port just pocking their nose into the port reciving free water (is it really social cooperation?).
>> **Solution:** Port use limit and Inter-trial interval.
>>> **Explanation:** Port use limit will work to force mice to change ports so we can start seeing the cooperation when they move to the other pair of ports. Inter-trial interval will try to prevent mice of being aware of a limited port use by setting a "long enough time" for the mouse get away from the port (lose interest), in that way we could decrease the go-and-come pattern.
>>> 3. **Lazy & Go-and-come behavior:** This behavior was observed on the alternate experiment, it showed up when the mice mixed the lazy behavior and the Go-and-come pattern. One mouse stick to a port while the other one start performing the Go-and-come pattern, in this way the one performing the Go-and-come pattern take advantage of the next port after fail parameter (in "alternate" mode) failing a trial and winning the one where the other mouse is poking. See illustration below.![[Lazy&Go-and-come.png|400]]
>>>>**Solution:** Next port after fail (Value: fixed).
>>>>> **Explanation:** A values of "fixed" for the next port after fail parameter means that the next port available will changed (chosen randomly) only when the mice win the trial (get reward). In that way, we force the mice go together to find the available pair of port and we avoid the emerged of the lazy & Go-and-come behavior.

## Predictions

+ This section describes my predictions for this experiment. This is the base that support the prosperity of my proposal. Are my results different from the ones of the alternate experiment? What kind of result do I expect?

>  **Marked difference between perforate and solid barrier:** Given the decrease of the ease to grasp a pattern, I would expect a worst performance in the solid barrier compared with the perforate barrier, since would be harder to synchronize their movements to discover the available port.
>  
>  **Less performace in all assays compared with the alternate experiment in early stages:** Since mice won't know what port is available, probably they will achieved less successful trials in the same time during the early stages.
>  
>  **Delayed learning:** Maybe mice could learn the mechanism's functionality in a slower rate than with the alternate experiment.

## Experimental design

+ Refer to this document to see the [[Experimental design]].