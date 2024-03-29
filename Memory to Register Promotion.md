---
created: 2023-09-08T14:31
updated: 2023-10-18T08:42
---
#compilers #programming 
[[Compiler Optimization|Compiler optimization]] with the following goals:
- Create more opportunity to optimize
- Replace slower [[Memory|memory]] operations with faster [[Register|register]] operations

## Prerequisites
C/C++ puts local [[Variable|variables]] in stack memory by default. However, variables can be moved into a register under the following conditions ([[Unambiguous Variable]]):
- We never need to know the variable’s address (Registers don’t have an address, and some code (like scanf) relies on knowing an address)

>[!note] In LLVM IR
>We can prove that an alloca is unambiguous iff it is only used in loads and stores as the address operand.