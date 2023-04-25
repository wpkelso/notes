#compilers #compiler_optimizations 
Useful in the context of [[Dead Code Elimination]], [[Instruction Scheduling]], and [[Register Allocation]]. 

>[!info] Definition
>A [[Register|register]] $r$ is considered ‘live’ at instruction $i$ if it is used by some instruction $j$ that is reachable from $i$ in the [[Control Flow Graph|CFG]].

Following this definition a register is considered ‘dead’ at $j$ if it is no longer used after $j$.

**Register Live Range:** a register’s live range is considered to be the range of instructions from its first definition until its final use.

## Computing Liveness
$$\text{livein}[i]=\text{use}[i]\cup (\text{liveout}[i]-\text{def}[i])$$
$$\text{liveout}[i]=\cup_{x=\text{succ}(i)}\text{livein}[x]$$
where:
- $\text{livein}[i]$ is the set of all registers live before executing $i$
- $\text{liveout}[i]$ is the set of all registers live after executing $i$
- $\text{use}[i]$ is the set of all registers used at $i$
- $\text{def}[i]$ is the set of all registers defined at $i$