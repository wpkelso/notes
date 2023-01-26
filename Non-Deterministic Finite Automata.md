#compilers #automata 
An example of a [[Finite Automata|finite automata]] where multiple edges with the same symbols are allowed to leave a state. Generally, these are bad for computers because they would have to guess which way to go on a transition. However, they are helpful for representing a large class of regular expressions.

>[!important] 
>NFAs have a special input, $\epsilon$. This means "no input" and an NFA is allowed to take an $\epsilon$-transition at any time.

![[Pasted image 20230124212520.png]]
0 or more repetitions on any NFA in the above fashion are known as a Kleene Closure.

![[Pasted image 20230124212540.png]]
*An example of alternation ("or") using $\epsilon$ edges*