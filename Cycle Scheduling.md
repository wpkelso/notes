#compilers 
A [[Instruction Scheduling|instruction scheduling]] methodology in which the ‘ready cycle’ (clock cycle in which each instruction is becomes ready to execute) is computed for each instruction, subject to [[Data Dependence|dependence]] and [[Computer Processor|resource]] constraints. These resource constraints are dealt with on a first-come-first-serve basis; if more than one instruction is ready to use the same resource at the same time, a priority hierarchy must be established.

## Algorithm
1. Build a [[Data Dependence Graph|data dependence graph]]
2. Use a [[Heuristic|heuristic]] to sort the graph into a linear ordering
3. Based on type of dependence:
	1. **True:** The ready cycle is the maximum between the current ready cycle and the dependence latency plus the ready cycle
	2. **Anti:** The ready cycle is the maximum between the current ready cycle and the dependence cycle
	3. **Output:** The ready cycle is the maximum between the current ready cycle and dependence cycle + the maximum of 1 and the difference between that latency of the instruction and the dependence plus 1
4. Schedule the instruction in the current cycle, then delete the instruction from the list

## Ordering Heuristics
- [[Data Dependence Height]]: A measure of how many dependences must be traversed to reach the end of the data dependence graph.
- [[Data Dependence Depth]]: Figures out the earliest point in time that an instruction could start execution.
- [[Slack]]: The difference between the depth and the height.
*Note: the heuristics can create orders that violate data dependencies, they act more as suggestions rather than controlling scheduling.*