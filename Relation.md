---
tags: [mathematics, set_theory]
---
# Relation

## Mathematics

In mathematics a relation is defined on a [[Set|set]] as a subset of ordered pairs sharing a certain quality ($x \leq y$, etc).

### Properties

- **Reflexivity:** For any $x$, $\left< x,x \right>\in R$
- **Transitivity:** For any $x, y$, if $\left< x,y \right>, \left< y,z \right>\in R$, then $\left< x,z \right> \in R$
- **Symmetry:** For any $x,y$ if $\left< x,y \right> \in R$, then $\left< y,x \right> \in R$.
- **Anti-Symmetry:** For any $x,y$ if $\left< x,y \right>\in R,\left< y,x \right>\in R \text{, then}\, x=y$
- **Asymmetry:** No $x,y \in A$ is in both $\left< x,y \right>,\left< y,x \right>\in R$. Naturally, a relation is asymmetric iff it is anti-symmetric and irreflexive.
- **Irreflexive:** For any $x \in A,\left< x,x \right> \notin R$

### Types of Orders

#### Equivalence Relation

A relation $R \subseteq A^2$ is considered an equivalence relation iff it is reflexive, symmetric, and transitive.

#### Partial Order

A relation $R \subseteq A^2$ is considered a partial order iff it is reflexive, anti-symmetric, and transitive.

#### Strict Order

A relation $R \subseteq A^2$ if considered a strict order iff it is irreflexive, asymmetric, and transitive.
