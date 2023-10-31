---
tags:
  - mathematics
  - programming
  - logic
created: 2023-09-22T15:24
updated: 2023-10-17T17:48
---

# Function

In mathematics, a function $f:A\to B$ is defined as a mapping of each element of A to an element of B.

>[!note] Definition
>$A$ is the **domain** of $f$, while $B$ is the **codomain** of f.

## Kinds of functions

### Surjective Function

A function is surjective iff $B$ is also the range of $f$. In other words, every object in $f$‘s codomain is the value of $f(x)$ for some input $x$.

### Injective Function

A function is injective iff for each $y\in B$ there is at most one $x\in A$ such that $f(x)=y$. To show that $f$ is an injection, show that for any elements $x$ and $y$ of $f$‘s domain, if $f(x)=f(y)$, then $x=y$.

### Bijective Function

A function is bijective iff it is both surjective and injective. As such, bijections pair elements in a one-to-one correspondence. 

### Graphs of Functions

The [[Graph|graph]] of a function is defined for $f:A \to B$ as the relation $R_{f} \subseteq A \times B$ defined by $R_{f}= \{ \langle x,y \rangle : f(x) = y \}$.