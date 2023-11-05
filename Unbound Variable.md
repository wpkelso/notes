---
aliases: Free Variable
tags: discrete_mathematics, logic, mathematics
created: 2023-10-24T17:36
updated: 2023-11-03T16:57
---

# Unbound Variable

In [[Predicate Logic]] and when considered as a part of a [[First-Order Language]], an unbound or “free” [[Variable|variable]] is a variable that is not bound by a quantifier such as $\forall$ or $\exists$.

They are defined [[Mathematical Induction|inductively]] by the following:

1. If $A$ is atomic, then all variable occurrences in $A$ are free
2. If $A$ is of the form $\lnot B$, then the free variable occurrences of $A$ are exactly those of $B$
3. If $A$ is of the form $B * C$, where $*$ is any of $(\land, \lor, \to)$, then the free variable occurrences of $A$ are exactly those of $B$ along with those of $C$
4. If $A$ is of the form $\forall v B$ or $\exists v B$, then the free variable occurrences of $A$ are all of those in $B$ **except for** occurrences of B

> [!note]
> A variable within a formula can have both _free_ and _bound_ occurrences, therefore it is more useful to talk about variable _occurrences_ in a formula, rather than just variables
