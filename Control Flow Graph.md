#compilers #programming

The Control Flow Graph is an important and widely used [[Hybrid Intermediate Representation|hybrid IR]]. As its most basic, it is a [[Directed Cyclic Graph|directed cyclic graph]] that represents control flow in the program. [[Vertex|Nodes]] are sets of **guaranteed sequential** instructions called "basic blocks." If control can flow from one basic block to another, an [[Edge|edge]] connects them. Basic blocks are then terminated by a branch.

## Creation
Starting from a linear sequence of instructions, 
1. Start a new block at the beginning of a function.
2. Terminate a block at any kind of branch instruction, typically excluding function calls
3. Start a new block at the destination of every branch

You can also leverage the [[Parse Tree|parse tree]] to build the control flow graph. This is really just another form of [[Semantic Analysis|syntax directed translation]].

## Properties
- [[Control Flow Dominance|Dominance]]
- [[Control Flow Post-Dominance|Post-Dominance]]
- [[Control Flow Loops|Loops]]