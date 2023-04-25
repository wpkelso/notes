#compilers #compiler_optimizations 
Useful in the context of [[Dead Code Elimination]], [[Instruction Scheduling]], and [[Register Allocation]]. 

>[!info] Definition
>A [[Register|register]] $r$ is considered ‘live’ at instruction $i$ if it is used by some instruction $j$ that is reachable from $i$ in the [[Control Flow Graph|CFG]].

Following this definition a register is considered ‘dead’ at $j$ if it is no longer used after $j$.

**Regi**