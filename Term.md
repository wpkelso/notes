---
tags: mathematics, logic, language
created: 2023-10-31T12:14
updated: 2023-10-31T13:11
---

# Term

In a [[First-Order Language|first-order language]] $\mathscr{L}$, a term is considered to be defined by the following:
1. Every variable is a term
2. Every constant symbol is a term
3. If $f$ is an $n$-place function symbol and $t_{1}, \dots, t_{n}$ are terms, then $f(t_{1},\dots,t_{n})$ is a term
4. Nothing else is a term

>[!note] 
>A *closed term*  is defined as a term containing no variables

These define [[Mathematical Induction|inductively]] all possible terms in the language.

## Free Term
Naturally, if [[Unbound Variable|variables can be unbound]], terms can as well.
>[!summary] Definition
>A term $t$ is free for $v$ in $A$ iff none of the variables in $t$ becomes bound if we substitute $t$ for all free occurrences of $v$ in $A$