---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#computer_architecture #programming 
## Conditional Branches
```asm
BEQZ R1 #label
```
Conditional branches move control based on the value in the [[Register|register]] specified. The *label* is an offset from the next instruction (relative offset)

## Unconditional Branches (Jumps)
```asm
JUMP #label
```
The jump instruction also uses the *label* as a relative offset