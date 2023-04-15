#compilers #computer_hardware 

## Predicted-not-taken
Continues to [[Datapath Design|fetch]] [[Instruction Set Architecture|instructions]]. If taken, discard the fetched instruction.
## Predicted-taken
## Backward taken, forward not taken
## Branch Delay Slot
Works well for a 5-stage [[Pipelining|pipeline]]. Moves code that will always be executed (independent of the [[Control Flow Instructions|branch]]) into the delay space where the outcome of the branch is unknown
## Profile-based
Provide individual branch ‘hints’ based on expected inputs