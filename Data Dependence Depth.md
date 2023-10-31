---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#compilers 
A [[Heuristic|heuristic]] that figures out the earliest point in time that an instruction could start execution, assuming latency of instructions and [[Data Dependence Graph|DDG]]. Data dependence depth ignores any limitations of the [[Computer Architecture|architecture]]. Essentially an opposite to [[Data Dependence Height]].

>[!important] Main Idea
> Prioritize instructions that can start earlier

>[!example] 
>![[Pasted image 20230417161956.png]]
>*If, like in the example above, multiple instructions have are considered as equal with respect to depth, the easiest way to order is just to use program order.*
