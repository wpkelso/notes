#compilers #compiler_optimizations

>[!summary] Idea
>Hoist loop invariant control flow out of a loop to simplify the loop

## Tradeoffs
**Advantages:** eliminates unnecessary conditional branches from each execution of the loop, creating fewer dynamic instructions which creates a direct impact on program performance. It also creates greater chances for other optimizations.
**Disadvantages:** unswitching branches can double the loop’s static size, potentially creating exponential growth (very dangerous). Loop unswitching also means that loops occupy more space in the instruction [[Cache|cache]].

## [[Algorithm]] 
1. Identify all loop invariants
2. If a conditional expression is based on an invariant:
	- If the overall size of the loop is small (<threshold instructions) then perform loop unswitching
		1. Move the conditional outside of the loop
		2. Create two copies of the loop, one with the then statements and one with the else statements
		3. reconnect the [[Control Flow Graph|CFG]] appropriately