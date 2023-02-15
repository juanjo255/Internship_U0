#ExperimentDescription

+ This document is a descriptive report of the seek-and-find proposal. It describes all about how could this proposal achieve the purpose of the social cooperation project.
+ If this proposal is approved or taking into account, the idea with the experimental design would be build it from the same template established for the "traditional" approach, but with a few differences.
+ Here I refer to the normal or traditional experiment as the "alternative experiment" and to my proposal as the "randomized experiment" or seek-and-find experiment.
----


```toc
```


----



## Philosophy

+ This section describes the reasoning behind the Seek-and-find experiment.

> The state that this approach want to achieve is that, once mice are by their own (lights turned off), they would have to coordinate each other to find the available port, once mice discover the available pair of ports a new pair of port will be selected randomly after n seconds. the need for coordinate their movements in order to find the available pair of ports will make harder to find the available pair of ports the more isolated they are. 


## Objectives

+ This section describes the specifics objectives that need to be follow in order to achieve the general objective of the social cooperation.

### Specific objectives 

> 1. Through ligth signaling, mice have to learn to receive water using their corresponding ports.
> 2. Through light signaling, mice have to learn to receive water using their corresponding port at the "same time" (during a limited period of time once a trial has started).
> 3. Mice have to be able to receive water using their corresponding port at the "same time" (during a limited period of time once a trial has started) without the help of the experimenter (lights).
> 4. Mice must show a decrease in *performance* receiving water when they are mutually isolated, that is, when they have lost any kind of "sense" of each other. 

### General objective

> + Identify evidence of social cooperation through the use of the proposed mechanism.

## Key points

+ This section describes the points that makes this proposal different from the alternate experiment.

> 1. **Random use of lights:** This method is used for train the mice in the alternate experiment. During this experiment lights will fulfill the same objective, except that they will indicate the availability of a port not in an alternate behavior but a random behavior (the pair of ports to be open will be random).  
> 2. **Limited use of ports:** This method will add this new hyperparameter. This hyperparameter will limit the times a port can be use in a row, in such a way we would force the move of the mice. The parameter has to be established over a value of 2, otherwise we would repeating the behavior of the alternate experiment. This port limitation will be taught during the appearance of the light, that is, a pair of light cannot be turned on more than n in a row, where n >= 2. In other words, the same pair of ports will not be available more than n times in a row.
> 3. **Inter-trial interval:** This is the same hyperparameter as the alternate experiment, but, unlike the aforementioned, in this experiment it will be use in the early stages, in order to give time mice to get away from the port (lose interest) and avoid the lazy behavior. This variable produces a windown of n seconds where nothing happens.
> 4. **Next port after fail:** The alternate experiment had this parameter established as "alternate", which means that if a mouse activate a trial regardless of if they win or fail (that is they do or not get the reward) the available pair of port changed to the next ones (from north to south and vice versa). In the Seek-and-find experimente this parameter will be established as "fixed", which means that the available pair of port will be choose (randomly) again only if mice win (get the reward).


## Troubleshooting

This section describes the problems the Seek-and-find experiment face so far and the solution that this approach gives for each of them. The problems can belong to the alternate experiment or could emerged with the randomized experiment.

### Go-and-come pattern: 

This problem can make the experiment questionable, given that between, for example, for perforate and solid barrier there are barely differences (results with a solid performance of 59% and perforate performance of 59% during same stages), which does not seem to be convincing. Basics statistics say that every mice pair by chance have only 25% of success in every trial (is it really social cooperation?). Look illustration below:
>>  ![[Go-and-come.png | 400]]
>> **Solution:** Random use of lights.
>>> **Explanation:** Using random use of light we avoid inducing patterns in mice which overshadows social cooperation, if a pattern arised, it would be an independent learnt pattern.

### The lazy behavior:

> This behavior can make questionable our experiment as much as the Go-and-come pattern, it concists of the mice sticking to a port just pocking their nose into the port reciving free water (is it really social cooperation?). Look illustration below:
>> ![[lazy.png|400]]
>> **Solution:** Limited use of ports and Inter-trial interval.
>>> **Explanation:** Limited use of ports will work to force mice to change ports so we can start seeing the cooperation when they move to the other pair of ports. Inter-trial interval will try to prevent mice of being aware of a limited port use by setting a "long enough time" for the mouse get away from the port (lose interest), in that way we could decrease the go-and-come pattern.

### Lazy & Go-and-come behavior:
>This behavior was observed on the alternate experiment, it showed up when the mice mixed the lazy behavior and the Go-and-come pattern. One mouse stick to a port while the other one start performing the Go-and-come pattern, in this way the one performing the Go-and-come pattern take advantage of the next port after fail parameter (in "alternate" mode) failing a trial and winning the one where the other mouse is poking. See illustration below.![[Lazy&Go-and-come.png|400]]
>>>>**Solution:** Next port after fail (Value: fixed).
>>>>> **Explanation:** A values of "fixed" for the next port after fail parameter means that the next port available will changed (chosen randomly) only when the mice win the trial (get reward). In that way, we force the mice go together to find the available pair of port and we avoid the emerged of the lazy & Go-and-come behavior.
### Hard learning
> + **I was thinking that could be difficult to mice jump from the stage 1 to stage 2** where stage 1 teachs them to use ports and immediately stage 2 force them to discover the available pair of ports and receive reward together.
>> + **Possible solution:** Maybe mice will need an extra stage before stage 2 same as this but with lights turning on indicating availability of port and not releasing water until they both arrive to the borth within a time window once a trial has started.

### Desperate behavior

> + I was thinking that the inter-trial interval might give them **despair** since nothing happens during that time. That could be leading them to not focus on the purpose of the task, which is to find the available port together after a period of time has passed, therefore they do not learn or learn take much time.
>> + **Possible solution:** Maybe during early stages, turn all lights on during the inter-trial interval in a static mode o flashing mode (maybe this could produce a stress state), in order to teach them that their is a moment of nothing happening.


### Incomplete isolation

>  + **This is more a futuristic concern.**
>  + Do they can hear each other through the solid barrier? In some of the videos I watched I noticed that during the solid barrier they were almost like capable of arrive to the same side as their partner, could be only coincidence, but I started suspect that they can hear each other and that is a kind of communication.


### Criteria to move to the next stage

> + **Precedent (Brigid):** Criteria for moving to the next stage were developed by first estimating what approximate performance would demonstrate that the mice had mastered the task they are on. After that, adjustments were made based on what level the mice actually were able to perform at in a realistic amount of time. In summary, the criteria for moving from one stage to another should allow for the mice to fully learn the stage they are on. If you are changing parameters there will probably be some guesswork and you will probably have to experiment to find the right criteria for moving to the next stage.
> + **My thinking:** **How would I estimate the criteria for move forward?** using the collected data, I would compute the mean of the rewards obtained by each mouse in stage 1 (since there they are working alone), then if they are working together we can assume them as single individual, so the theorical estimation would be that, to move to the next stage, they would have to achieve in average a number of rewards similar to the computed for stage 1 **(The question then would be how much difference can be between both values? (standard deviation?? t-test??))** However, all is behavior-dependent. Likewise, we can plot a line graph like the below, in which we can see an increase over the days of training and set a limit when an asymptote appears. Lets see an example:
> ![[means.png]]
> + **The image above shows three means from 3 different stages (from stage 1 to 4 from top to bottom, stage 3 ignored). similar values?** 
> ![[coop.png]]
> + **The image above shows a line graph evaluating the learning through time, using days (x axis) and mutual rewards (y axis).** 
> + **(I am just rambling now, this would be applied to move from stage 2)** this approach is hard to see in brigid's data, because of the go-and-come patter that was taught since stage 1, however reasoning goes as follow: When comparing the first day of training of each stage with any of the next days we have to see an increment close to the 25% (if they are not working together as in the first day of training, each mouse has 50% of reaching the correct port and to receive the reward together they have 25%. If they start to work together assuming that they are a same individual they will have chances of 50% to get the reward. Then, increment of 25%). **Lets see some examples in brigids data**
![[Pasted image 20230214153904.png]]
> In the image above, from **2022-11-04** onwards, we can see increases of up to 23%.

----


## Experimental design

+ This document describes the experimental design that will be apply to achieved the objectives of the social cooperation project escribed in [[Seek-and-find approach description]] document.
----

### General points
> + This section describes the points that all stages fullfill.  
>>  + Inter-trial interval is only applied if mice achieve a successful trial.
>>  + A new randomly pair of ports is selected only if mice achieve a successful trial.
>>  + Limited use of ports is established in all stages, that is, a port will not be available more than n times in a row.


---
### Training stages

+ This section describes each training stage need for achieve social cooperation project goal.
+ Training will concist of 4 stages with the same organization as in the alternate experiment.


----

#### Stage 1

##### Objectives

> ###### General objective
> + Familiarize mice with ports and reward systems using lights.
> ###### Specifics objectives
> + Mouse has to insert their nose into the port when the light turns on (controlled by experimenter) to obtain reward (water).
> + Both mice can get their reward if they insert their nose into the port when the light is turned on. 


##### Detail description

> + Two mice at the same time (on different tracks).
> + To get reward, a mouse has to insert its nose into a port while the light is on.
> + Either mice or both mice can obtain a reward.
> + Two lights on the same randomly selected side will turn on at the same time indicating the available port to get the reward (water).
> + **The light will turn on for 3 seconds, after that time will be a 3 seconds timeout (Inter-trial interval) only if it has been successful (mouse get the reward). A new side will be selected randomly only if a mouse get the reward, otherwise the same side will turn on**.
> + **Criteria for moving to next stage: Mice must spend three training sessions on this stage as well as have 800 initiated trials minimum per day.** Next Stage: [[Stage 2]].

##### Set parameters

> + Session Info: default
> + Water delivery: 0.03 sec
> + **Limited port use**: 3
> + Timing parameters:
>> + Wait time: 3 sec
>> + **Inter-trial interval:** 3 sec
> + General parameters:
>> + Barrier type: perforated
> + Task mode: auto_lights
> + **Next port after fail:** Fixed


----

#### Stage 2

##### Objectives

> ###### General objective
>> + Teach mice to synchronize port activation for reward (using lights).
> ###### Specific objective
>> + Mice must coordinate poking of ports to obtain reward within 3 second window (Task mode: Reward_on_last_poke). Lights are turned on when either of the mice start a trial inserting its nose into the available port on the randomly chose side.


##### Detail description

> + The first trial will be in the ports of a randomly selected side of the rig. Thereafter, the side with the available pair of ports  will continue to be randomly selected.
> + A trial starts with the mouse inserting first its nose into the port of the available side (north or south) chosen randomly, then both lights bulbs on the same side will turn on for 3 seconds and the other mouse will have that time to reach it and obtain a reward.
> + **Once one of them has initiated a trial, a reward will only be given for both if they both insert their nose into the ports on the same side within the 3 seconds they are granted (successful trial, otherwise, failed trial). See graphical demostration bellow.**
>  ![[success_3secs_stages.png | 400]]
> + After the 3 second period when ligths are off, only if they achieve a successful trial a Inter-trial interval (3 sec) will applied and a new side will be chosen randomly, otherwise the same side will turn lights on again immediately.
> + **Criteria for moving to next stage: 500 initiated trials for 3 consecutive days with greater than 50% rewarded.** Next Stage: [[Stage 3]].



##### Set parameter

> + Session Info: default
> + Water delivery: 0.03 sec
> + **Limited port use**: 3
> + Timing parameters:
>> + Wait time: 3 sec
>> + **Inter-trial interval:** 3 sec
> + General parameters:
>> + Barrier type: perforated
> + Task mode: reward_on_last_poke
> + **Next port after fail:** Fixed


----


#### Stage 3

##### Objectives

> ###### General objective
>> + To teach mice to synchronize port activation for reward without light as a stimulus (LED will still flash when reward is granted to both mice)
> ###### Specific objective
>> + Mice must coordinate poking of ports the obtain reward within 3 second window (Task Mode: cooperate). Only if mice get the reward, next available pair of ports is selected randomly, otherwise stay the same.


##### Detail description

> + A trial starts with the mouse inserting firts its nose into the port of the side (north or south) chosen randomly to be available.
> + **Once one of them has initiated a trial, a reward will only be given for both if they both insert their nose into the ports on the same side within the 3 seconds they are granted  (successful trial, otherwise, failed trial). See graphical demostration bellow.**
> ![[success_1sec.png | 400]]
> + The first trial will be in the randomly selected side of the rig. Thereafter, the side with the available port pair will continue to be randomly selected.
> + After the 3 second period regardless of whether a reward was given or not, mice have to wait 3 second before try again. A new side will not be chosen randomly again until mice achieve a successful trial.
> + **Criteria for moving to next stage: 500 initiated trials for 3 consecutive days with greater than 50% rewarded.** Next Stage [[Stage 4]].

##### Set parameters

> + Session Info: default
> + Water delivery: 0.03 sec
> + **Limited port use**: 3
> + Timing parameters:
>> + Wait time: 3 sec
>> + **Inter-trial interval:** 3 sec
> + General parameters:
>> + Barrier type: perforated
> + Task mode: cooperate
> + **Next port after fail:** Fixed

----


#### Stage 4

##### Objectives

> ###### General objective
>> + To teach mice to synchronize port activation in a shorter time period for reward without light as a stimulus.(LED will still flash when reward is granted to both mice).
> ###### Specific objective
>> + Mice must coordinate poking of ports to obtain reward within 1 second window (Task Mode: cooperate).

##### Detail description

> + A trial starts with the mouse inserting first its nose into the port of the available side (north or south) selected randomly.
> + **Once one of them has initiated a trial, a reward will only be given for both if they both insert their nose into the ports on the same side within the 1 seconds they are granted  (successful trial, otherwise, failed trial).**
> + The first available pair of ports will be in the side of the rig selected randomly. Thereafter, the side with the available port pair will continue to be randomly selected.
> + Only if mice achieve a successful trial the Inter-trial interval (3 sec) will be applied and a new pair of ports will be selected to be available.
> + **Criteria for moving to next stage: 500 initiated trials for 3 consecutive days with greater than 50% rewarded(we were unable to achieve this, consider moving boundary for moving to next stage downward)**

##### Set parameters

> + Session Info: default
> + Water delivery: 0.03 sec
> + **Limited port use**: 3
> + Timing parameters:
>> + Wait time: 1 sec
>> + **Inter-trial interval:** 3 sec
> + General parameters:
>> + Barrier type: perforated
> + Task mode: cooperate
> + **Next port after fail:** Fixed


----

## Predictions

+ This section describes my predictions for this experiment. This is the base that support the prosperity of my proposal. Are my results different from the ones of the alternate experiment? What kind of result do I expect?

>  **Marked difference between perforate and solid barrier:** Given the decrease of the ease to grasp a pattern, I would expect a worst performance in the solid barrier compared with the perforate barrier, since would be harder to synchronize their movements to discover the available port.
>  
>  **Less performace in all assays compared with the alternate experiment in early stages:** Since mice won't know what port is available, probably they will achieved less successful trials in the same time during the early stages.
>  
>  **Delayed learning:** Maybe mice could learn the mechanism's functionality in a slower rate than with the alternate experiment.

----

## Results

> + **How do we know our experiment success, in other words, how can we know that mice are cooperating?**
>> Well, using the approach of perforate barrier and solid barrier, we should see a **decrease** in the rewards obtained in isolation (solid barrier) compared with access to most senses (perforate barrier).
> + **How do we show that decreasing?**
>>  I propose to use the bar chart. **Why?** because this plot let me compare a numerical variable (acummulated rewards or average rewards obtained) measured in different categorical variables (solid and perforate barrier). 
>>  **Example of a bar chart:** 
>>>  In this case we would change performance for average mutual regard or accumulated rewards. **Why?** because we standarized by time (1 hr a day). How many rewards they can achieved in 1 hr? 
>>>  The initiation of a trial is subject to the behavior of every mice (what if one is thistier than the other one?), so to compute by performance we would have to standarized by trials (?), which is harder, because if one mouse started initiating many trials and the other is not coopering then the performance would be lower and I think it is a bias.
>>>  **Example:** 
![[Screenshot 2023-02-13 at 10.21.59 AM.png | 400]]




