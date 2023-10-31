---
created: 2023-09-08T14:31
updated: 2023-10-18T08:42
---
#computer_architecture 
The intention is to design a data path for a specific [[Instruction Set Architecture|instruction set architecture]].

## Life of an Instruction
1. **Instruction Fetch:** Fetch one instruction from [[Memory|memory]] & store it in a special-purpose [[Register|register]] - uses the [[Instruction Memory]]
   *All instructions use this stage*
2. **Instruction Decode:** Decode the instruction - [[Register File]]
	1. Look at the opcode
	2. If required, read the register file
	*All instructions use this stage*
3. **Execute:** Execute the instruction - use the [[Arithmetic Logic Unit|ALU]] to execute the [[Arithmetic Instructions|arithmetic operation associated with the instruction.]]
   *Arithmetic instructions use this to compute the result, and [[Memory Instructions|memory instructions]] use this to compute the address to write to. branches*
4. **Memory:** Memory access - uses [[Memory|data memory]]
   *LOAD/STORE use this stage*
5. **Writeback:** Write the result in the register file - [[Register File]]
   *Arithmetic operations & LOAD use this stage*
