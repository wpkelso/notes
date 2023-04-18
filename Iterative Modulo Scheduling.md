#compilers #computer_architecture #programming 
An [[Instruction Scheduling|instruction scheduling]] methodology in which instructions are placed into a scheduling window, obeying [[Data Dependence|dependences]] and [[Computer Processor|resource constraints]].

## Approach
1. Guess at the length of schedule and then try to fit the [[Instruction Set Architecture|instructions]] into that scheduling window, obeying dependences and resource constraints
2. If it doesn’t work, try a longer length

## Guessing the Schedule 
**Initiation Interval (II):** Number of cycles between the start of each iteration
**Minimum Initiation Interval (MII):** Theoretically lowest II possible
- Constraints on schedule length: resources and data dependence cycles
	- RecMII: recurrence based MII (data dependence cycles)
	- ResMII: resource based MII
- $\Delta$ = MII = max(ResMII, RecMII)
*Try to schedule with $\Delta$=MII. If that doesn’t work try $\Delta=\Delta+1$*

### Finding ResMII
Ignore dependences and calculate minimum schedule length given resources.
>[!note] Approximation
>1. For each Functional Unit type, calculate $$\text{ResMII}_\text{Type}=\text{Num of Inst}_\text{Type}/\text{Num of Units}_\text{Type}$$
>2. ResMII = max(ResMII of all Functional Units)

### Finding RecMII
Circular dependence between iterations determines schedule length–like the maximum slope in ideal loop pipelining
>[!note] Approximation
>1. For each dependence cycle, length = sum of dependence latencies in the cycle
>2. RecMII = max(cycle length of all cycles)