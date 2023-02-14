+ This document describes everything in detail related with the **Stage 3**.

# Objectives

> ## Specific objective
>> + Mice must coordinate poking of ports to obtain reward within 3 second window (Task Mode: cooperate).
> ## General objective
>> + Teach mice to synchronize port activation for reward without light as a stimulus (LED will still flash when reward is granted to both mice)

# Detail description

> + A trial starts with the mouse inserting firts its nose into the port of the side (north or south) chosen randomly to be available.
> + **Once one of them has initiated a trial, a reward will only be given for both if they both insert their nose into the ports on the same side within the 3 seconds they are granted  (successful trial, otherwise, failed trial). See graphical demostration.**
> + The first trial will be in the randomly selected side of the rig. Thereafter, the side with the available port pair will continue to be randomly selected.
> + After the 3 second period regardless of whether a reward was given or not, mice have to wait 3 second before try again. A new side will not be chosen randomly again until mice achieve a successful trial.
> + **Criteria for moving to next stage: 500 initiated trials for 3 consecutive days with greater than 50% rewarded.** Next Stage [[Stage 4]].

## Graphical demostration


![[success_1sec.png | 500]]

## Set parameters
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