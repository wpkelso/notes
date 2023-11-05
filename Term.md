---
tags: mathematics, logic, language
created: 2023-10-31T12:14
updated: 2023-11-03T17:14
---

# Term

In a [[First-Order Language|first-order language]] $\mathscr{L}$, a term is considered to be defined by the following:

1. Every variable is a term
2. Every constant symbol is a term
3. If $f$ is an $n$-place function symbol and $t_{1}, \dots, t_{n}$ are terms, then $f(t_{1},\dots,t_{n})$ is a term
4. Nothing else is a term

> [!note]
> A _closed term_ is defined as a term containing no variables

These define [[Mathematical Induction|inductively]] all possible terms in the language.

## Free Term

Naturally, if [[Unbound Variable|variables can be unbound]], terms can as well.

> [!summary] Definition
> A term $t$ is free for $v$ in $A$ iff none of the variables in $t$ becomes bound if we substitute $t$ for all free occurrences of $v$ in $A$

## Substitution

Given a term $s$, we can inductively define $s \left[ t/v \right]$, the result of *substituting the term $t$ for every occurrence of the variable $v$ in $s$* as follows:
- If $s$ is a constant $c$, then $s \left[ t/v \right]=c$
- If $s$ is a variable $v'$ different from $v$, then $s \left[ t/v \right]=s$
- If $s$ is identical to the variable $v$, then $s \left[ t/v \right]=t$
- If $s$ is of the form $f\left( t_{1}, \dots, t_{n}\right)$, then $s\left[ t/v \right]=f\left( t_{1}\left[ t/v \right],\dots,t_{n}\left[ t/v \right] \right)$