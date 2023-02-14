
+ This document describes the experimental design that will be apply to achieved the objectives of the social cooperation project escribed in [[Seek-and-find approach description]] document.

```toc
```

----
## General points
> This section describes the points that all stages fullfilled.  
>>  + Inter-trial interval is only applied if mice achieve a successful trial (meaning of successfull trial can change with each stage).
>>  + A new randomly pair of ports is selected only if mice achieve a successful trial.
>>  + Limited use of usage is established in all stages.
## Training stages

+ This section describes each training stage need for achieve social cooperation project goal.
+ Training will concist of 4 stages with the same organization as in the alternate experiment.


----



### [[Stage 1]]

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



### [[Stage 2]]

+ **Goal:** To teach mice to synchronize between them port activation for reward (through ligths).
+ **Task:** Mice must coordinate poking of ports to obtain reward within 3 second window (Task mode: Reward_on_last_poke). Lights turn on once a mouse has started a trial poking its nose into the available port on the randomly chose side. 
+ **Details and parameters:** [[Stage 2]]

----


### Stage 3

+ **Goal:** To teach mice to synchronize port activation for reward without light as a stimulus (LED will still flash when reward is granted to both mice)
+ **Task:** Mice must coordinate poking of ports the obtain reward within 3 second window (Task Mode: cooperate). Only if mice get the reward, next available pair of ports is selected randomly, otherwise stay the same.
+ **Details and parameters:** [[Stage 3]]

----


### Stage 4

+ **Goal:** To teach mice to synchronize port activation in a shorter time period for reward without light as a stimulus.(LED will still flash when reward is granted to both mice).
+ **Task:** Mice must coordinate poking of ports to obtain reward within 1 second window (Task Mode: cooperate).
+ **Details and parameters:** [[Stage 4]]



## Troubleshootings

### Hard learning

> + **I was thinking that could be difficult to mice jump from the stage 1 to stage 2** where stage 1 teachs them to use ports and immediately stage 2 force them to discover the available pair of ports and receive reward together.
>> + **Possible solution:** Maybe mice will need an extra stage before stage 2 same as this but with lights turning on indicating availability of port and not releasing water until they both arrive to the borth within a time window once a trial has started.

### Desperate behavior

> + I was thinking that the inter-trial interval might give them **despair** since nothing happens during that time. That could be leading them to not focus on the purpose of the task, which is to find the available port together after a period of time has passed, therefore they do not learn or learn take much time.
>> + **Possible solution:** Maybe during early stages, turn all lights on during the inter-trial interval in a static mode o flashing mode (maybe this could produce a stress state), in order to teach them that their is a moment of nothing happening.
>> + This will be applied only if I decide to establish a intermediate stage between stage 1 and 2.

### Incomplete isolation

>  + **This is more a futuristic concern.**
>  + Do they can hear each other through the solid barrier? In some of the videos I watched I noticed that during the solid barrier they were almost like capable of arrive to the same side as their partner, could be only coincidence, but I started suspect that they can hear each other and that is a kind of communication.


### Criteria to move to the next stage

> + **Precedent:** Criteria for moving to the next stage were developed by first estimating what approximate performance would demonstrate that the mice had mastered the task they are on. After that, adjustments were made based on what level the mice actually were able to perform at in a realistic amount of time. In summary, the criteria for moving from one stage to another should allow for the mice to fully learn the stage they are on. If you are changing parameters there will probably be some guesswork and you will probably have to experiment to find the right criteria for moving to the next stage.
> + **My thinking:** **How would I estimate the requirements for move forward?** I would mean the number of rewards obtained by each mouse in stage 1 (since there they are working alone), then if they are working together we can assume them as single individual, so the theorical estimation would be that to move to the next stage they would have to achieve a number of rewards similar (or less) to that computed mean. However, all is behavior-dependent. **(just rumbling now)** When comparing the first day of training of each stage with any of the next days we have to see an increment close to the 25% (if they are no working together as in the first day, each mouse has 50% of reach the correct port and to receive the reward together they have 25%. If they start to work together assuming that they are a same individual they will have chances of 50% to get the reward. Then, increment of 25%)

## Results

> + First of all we need to show that the training is working. To do that **we can compare the number of rewards achieved in each day** and plot that in a line chart. example: 
> ![[coop.png]]
> + **How do we know our experiment success, in other words, how can we know that mice are cooperating?**
>> Well, using the approach of perforate barrier and solid barrier, we should see a decrease in performance (% win trials) in isolation (solid barrier) compared with access to most senses (perforate barrier).
> + **How do we show that decreasing?**
>>  I propose to use the bar chart. **Why?** because this plot let me compare a numerical variable (average mutual rewards) measured in different categorical variables (solid and perforate barrier). 
>>  **Average mutal rewards=** sum of the rewards obtained in every day of evaluation divide by the number of evaluated days. Example: 
>>>  In this case we would change cumulative mutual rewards for average mutual regard. **Why?** because we standarized by time (1 hr a day). How many rewards they can achieved in 1 hr? 
>>> The initiation of the trial is subject to the behavior of every mice (what if one is thistier than the other one?), so to compute by performance we would have to standirized by trials (?), which is harder, because if one mouse started initiating many trials and the other is not coopering then the performance would be lower and I think is a bias.
![[Screenshot 2023-02-13 at 10.21.59 AM.png | 400]]
