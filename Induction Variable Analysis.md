#compilers #programming 
Induction variable analysis is the [[Algorithm|algorithm]] by which [[Induction Variables|induction variables]] are found within a program in [[Static Single-Assignment|SSA form]]. A major limit of this algorithm however is that it can only detect linear induction variables.

## Algorithm
1. Find all cycles in the SSA graph consisting of only a [[Phi-Node|phi-node]] and [[Arithmetic Instructions|add/sub]]. These are the ‘basic’ induction variables.
2. Find all variables $y$ that are defined once and in the form of an add/sub or mult/div operation involving an induction variable $z$ and a constant $K$. If $z$ is not basic but in the family of $x$ then $y$ is of the family of $x$, otherwise $y$ is of the family of $z$.