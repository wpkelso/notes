#compilers 
A form of organization for an [[Intermediate Representation|IR]] where all [[Register|registers]] are defined only once and never re-defined.

>[!note] Example
>```assembly
>%10 = add %8, %9
>%10 = add %10, %8
>%8 = sum %10, %9
>```
>becomes
>```assembly
>%10 = add %8, %9
>%10_1 = add %10, %8
>%8_1 = sum %10_1, %9
>```

Additionally, all definitions [[Control Flow Dominance|dominate]] their uses, except for in [[Phi-Node|phi-nodes]].

>[!important] Important Effects of SSA Form
>- Makes finding uses easier as there are no forward traversals of the [[Control Flow Graph|CFG]]
>- Makes finding a definition easier, as every register is unique and only has one definition
>- The presence or absence of [[Phi-Node|phi instructions]] will be useful for optimization, as phis will only show up in specific situations that outline important behaviors that should be optimized

## Dominance Property of SSA Form
Definitions **always** dominate uses, with the following two rules holding true:
- If register $x$ is used in a non-phi instruction in block $n$, then the definition of $x$ dominates $n$
- If $x$ is the  i-th argument of a phi-instruction in block $n$, then the definition of $x$ dominates the i-th predecessor of $n$.

## Approaches for Generating Code
There are two methods for generating code in SSA form:

1. Approach 1
	1. Generate code that is not in SSA-form
	2. Put phi-nodes into the program anywhere its required to merge definitions of registers
2. Approach 2
	1. Let the parser generate inefficient code that conforms trivially to SSA-form
	2. For C code this looks like putting all variables in [[Computer Memory|memory]] and generating loads and stores at all definitions; this will never require a phi-node
	3. Later optimization passes will move variables into registers for performance; SSA form must be obeyed when this is done