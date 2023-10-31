---
tags: mathematics, logic, discrete_mathematics, programming
created: 2023-09-25T09:07
updated: 2023-10-31T12:13
---

# Formula

>[!summary] Definition
>A concise, symbolic way of expressing information

## First-Order Language

The set of formulas for a [[First-Order Language|first-order language]] is defined—like the set of terms—inductively by the following:
1. $\bot$ is an atomic formula
2. If $R$ is an $n$-place predicate symbol and and $t_{1},\dots,t_{n}$ are terms, then $R(t_{1},\dots,t_{n})$ is an atomic formula
3. If $t_{1}$ and $t_{2}$ are terms, then $=(t_{1}, t_{2})$ is an atomic formula
4. If $A$ is a formula, then $\lnot A$ is a formula
5. If $A$ and $B$ are formulas, then so are $(A \land B), (A \lor B), (A \to B)$
6. If $A$ is a formula and $v$ is a variable, then so are $\forall v A$ and $\exists v A$
7. Nothing else is a formula

>[!info] 
>For ease, rule 2 and rule 3 are often written as $t_{1} R t_{2}$ and $t_{1}=t_{2}$ respectively