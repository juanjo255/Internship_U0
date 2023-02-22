
+ This document describes the experimental design that will be apply to achieved the objectives of the social cooperation project escribed in [[Seek-and-find approach description]] document.

```toc
```

----

## General points
> + This section describes the points that all stages fullfill.  
>>  + Inter-trial interval is only applied if mice achieve a successful trial (meaning of successfull trial can change with each stage).
>>  + A new randomly pair of ports is selected only if mice achieve a successful trial.
>>  + Limited use of ports is established in all stages, that is, a port will not be available more than n times in a row.


---
## Training stages

+ This section describes each training stage need for achieve social cooperation project goal.
+ Training will concist of 4 stages with the same organization as in the alternate experiment.


----

### Stage 1

#### Objectives

> ##### General objective
> + Familiarize mice with ports and reward systems using lights.
> ##### Specifics objectives
> + Mouse has to insert their nose into the port when the light turns on (controlled by experimenter) to obtain reward (water).
> + Both mice can get their reward if they insert their nose into the port when the light is turned on. 


#### Detail description

> + Two mice at the same time (on different tracks).
> + To get reward, a mouse has to insert its nose into a port while the light is on.
> + Either mice or both mice can obtain a reward.
> + Two lights on the same randomly selected side will turn on at the same time indicating the available port to get the reward (water).
> + **The light will turn on for 3 seconds, after that time will be a 3 seconds timeout (Inter-trial interval) only if it has been successful (mouse get the reward). A new side will be selected randomly only if a mouse get the reward, otherwise the same side will turn on**.
> + **Criteria for moving to next stage: Mice must spend three training sessions on this stage as well as have 800 initiated trials minimum per day.** Next Stage: [[Stage 2]].

#### Set parameters

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




----

### Stage 2

#### Objectives

> ##### General objective
>> + Teach mice to synchronize port activation for reward (using lights).
> ##### Specific objective
>> + Mice must coordinate poking of ports to obtain reward within 3 second window (Task mode: Reward_on_last_poke). Lights are turned on when either of the mice start a trial inserting its nose into the available port on the randomly chose side.


#### Detail description

> + The first trial will be in the ports of a randomly selected side of the rig. Thereafter, the side with the available pair of ports  will continue to be randomly selected.
> + A trial starts with the mouse inserting first its nose into the port of the available side (north or south) chosen randomly, then both lights bulbs on the same side will turn on for 3 seconds and the other mouse will have that time to reach it and obtain a reward.
> + **Once one of them has initiated a trial, a reward will only be given for both if they both insert their nose into the ports on the same side within the 3 seconds they are granted (successful trial, otherwise, failed trial). See graphical demostration bellow.**
>  ![[success_3secs_stages.png | 400]]
> + After the 3 second period when ligths are off, only if they achieve a successful trial a Inter-trial interval (3 sec) will applied and a new side will be chosen randomly, otherwise the same side will turn lights on again immediately.
> + **Criteria for moving to next stage: 500 initiated trials for 3 consecutive days with greater than 50% rewarded.** Next Stage: [[Stage 3]].



#### Set parameter

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


### Stage 3

#### Objectives

> ##### General objective
>> + To teach mice to synchronize port activation for reward without light as a stimulus (LED will still flash when reward is granted to both mice)
> ##### Specific objective
>> + Mice must coordinate poking of ports the obtain reward within 3 second window (Task Mode: cooperate). Only if mice get the reward, next available pair of ports is selected randomly, otherwise stay the same.


#### Detail description

> + A trial starts with the mouse inserting firts its nose into the port of the side (north or south) chosen randomly to be available.
> + **Once one of them has initiated a trial, a reward will only be given for both if they both insert their nose into the ports on the same side within the 3 seconds they are granted  (successful trial, otherwise, failed trial). See graphical demostration bellow.**
> ![[success_1sec.png | 400]]
> + The first trial will be in the randomly selected side of the rig. Thereafter, the side with the available port pair will continue to be randomly selected.
> + After the 3 second period regardless of whether a reward was given or not, mice have to wait 3 second before try again. A new side will not be chosen randomly again until mice achieve a successful trial.
> + **Criteria for moving to next stage: 500 initiated trials for 3 consecutive days with greater than 50% rewarded.** Next Stage [[Stage 4]].

#### Set parameters

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


### Stage 4

#### Objectives

> ##### General objective
>> + To teach mice to synchronize port activation in a shorter time period for reward without light as a stimulus.(LED will still flash when reward is granted to both mice).
> ##### Specific objective
>> + Mice must coordinate poking of ports to obtain reward within 1 second window (Task Mode: cooperate).

#### Detail description

> + A trial starts with the mouse inserting first its nose into the port of the available side (north or south) selected randomly.
> + **Once one of them has initiated a trial, a reward will only be given for both if they both insert their nose into the ports on the same side within the 1 seconds they are granted  (successful trial, otherwise, failed trial).**
> + The first available pair of ports will be in the side of the rig selected randomly. Thereafter, the side with the available port pair will continue to be randomly selected.
> + Only if mice achieve a successful trial the Inter-trial interval (3 sec) will be applied and a new pair of ports will be selected to be available.
> + **Criteria for moving to next stage: 500 initiated trials for 3 consecutive days with greater than 50% rewarded(we were unable to achieve this, consider moving boundary for moving to next stage downward)**

#### Set parameters

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

## Results

> + **How do we know our experiment success, in other words, how can we know that mice are cooperating?**
>> Well, using the approach of perforate barrier and solid barrier, we should see a **decrease** in the rewards obtained in isolation (solid barrier) compared with access to most senses (perforate barrier).
> + **How do we show that decreasing?**
>>  I propose to use the bar chart. **Why?** because this plot let me compare a numerical variable (acummulated rewards) measured in different categorical variables (solid and perforate barrier). 
>>  **Example of a bar chart:** 
>>>  In this case we would change performance for average mutual regard. **Why?** because we standarized by time (1 hr a day). How many rewards they can achieved in 1 hr? 
>>>  The initiation of the trial is subject to the behavior of every mice (what if one is thistier than the other one?), so to compute by performance we would have to standirized by trials (?), which is harder, because if one mouse started initiating many trials and the other is not coopering then the performance would be lower and I think it is a bias.
>>>  Example:
![[Screenshot 2023-02-13 at 10.21.59 AM.png | 400]]


## Metadata

coop010
