#computer_architecture 
A [[Pipelining|pipelined]] data-path that supports [[IEEE Floating-Point Representation|floating-point]] operations, through the use of floating-point [[Register|registers]] and floating-point [[Instruction Set Architecture|instructions]]. Of these instructions, there are 2 types: single precision (32-bit, .S) and double precision (64-bit, .D)

## Multi-Cycle Operations:
Assume 4 functional units:
1. Integer: loads, stores, Int [[Arithmetic Logic Unit|ALU]] ops, branches
2. FP adder
3. FP and integer multiplier
4. FP and integer divider
*The floating point units only handle [[Arithmetic|arithemetic operations]]*

## How all of this affects the pipeline
1. Multiple functional units in the [[Datapath Design|execution stage]]
2. Execution stage can now have a latency >1
	1. Different execution units can have different latencies
2. Execution units can be pipelined