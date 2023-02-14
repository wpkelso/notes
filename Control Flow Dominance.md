#compilers #programming 

>[!info] Formal Definition
>A block B in a [[Control Flow Graph|control flow graph]] is said to dominate a block C is all [[Path|paths]]from the start node to C must go through B.

This is written as *B dom C*, or when excluding the case of a block always dominating itself, *B strictly dominates C*.

## Immediate dominators
B immediately dominates C if B is the nearest dominator of C, written as *B idom C*. With this, you can create a [[Dominator Tree]]