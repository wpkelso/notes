#compilers 
A [[Heuristic|heuristic]] measure of how many dependences must be traversed to reach the end of the [[Data Dependence Graph|data dependence graph]]. This includes a notion of execution latency, [[Data Dependence|data dependence]], ignores the limitations of the [[Computer Processor|processor]], and means that earlier instructions have a greater height than later ones.

>[!important] Main Idea
> Instructions farthest from the end of the program get prioritized

## Calculation
Start at the end of DDG and working up the tree, attach values to instructions according to the latency of the instruction as well as it’s dependencies.

>[!example] 
>![[Pasted image 20230417161106.png]]