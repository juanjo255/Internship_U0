+ This document describes everything in detail related with the **Stage 2**.

# Objectives

> ## Specific objective
>> + Mice must coordinate poking of ports to obtain reward within 3 second window (Task mode: Reward_on_last_poke).
> ## General objective
>> + Teach mice to synchronize port activation for reward.

# Detail description

> + The first trial will be in the ports of a randomly selected side of the rig. Thereafter, the side with the available port pair will continue to be randomly selected.
> + A trial starts with the mouse inserting firts its nose into the port of the side (north or south) chosen randomly to be available, then both lights bulbs on the same side will turn on for 3 seconds and the other mouse will have that time to reach it and obtain a reward.
> + **Once one of them has initiated a trial, a reward will only be given for both if they both insert their nose into the ports on the same side within the 3 seconds they are granted (successful trial, otherwise, failed trial). See graphical demostration.**
> + After the 3 second period when ligths are off, regardless of whether a reward was given or not, mice have to wait 3 second before try again. A new side will not be chosen randomly again until mice achieve a successful trial.
> + **Criteria for moving to next stage: Mice must spend three training sessions on this stage as well as have 800 initiated trials minimum per day.** Next Stage: [[Stage 3]].


## Graphic demonstration


![[success_3secs_stages.png | 500]]

## Set parameter

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


