---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#compilers #computer_hardware 

## Predicted-Not-Taken
Continues to [[Datapath Design|fetch]] [[Instruction Set Architecture|instructions]]. If taken, discard the fetched instruction.

## Predicted-Taken

## Backward Taken, Forward Not Taken
The rationale behind this is that usually backwards branches will characterize loops, while forward branches will not. Therefore, predicting backwards branches to be loops and taking them will be correct most of the time, while preserving the efficiency of falling through on non-loops branches.

## Branch Delay Slot
Works well for a 5-stage [[Pipelining|pipeline]]. Moves code that will always be executed (independent of the [[Control Flow Instructions|branch]]) into the delay space where the outcome of the branch is unknown. This behavior needs to avoid placing branch instructions into the delay space, as such instructions could create an unclear behavior.
### How is this achieved?
The compiler must first determine a sequential successor.

## Profile-Based
Provide individual branch ‘hints’ based on expected inputs