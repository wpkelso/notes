#compilers #compiler_optimizations

>[!summary] Idea
>Hoist loop invariant control flow out of a loop to simplify the loop

## Tradeoffs
**Advantages:** eliminates unnecessary conditional branches from each execution of the loop, creating fewer dynamic instructions which creates a direct impact on program performance. It also creates greater chances for other optimizations.
**Disadvantages:** Unswitching branches can double the loop’s static size, potentially creating exponential growth (very dangerous). Loop unswitching also means that loops occupy more space in the instruction [[Cache|cache]].