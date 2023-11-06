---
aliases: Structure
tags: mathematics, discrete_mathematics, logic
created: 2023-10-31T13:24
updated: 2023-11-06T10:48
---

# Model

A model in a [[First-Order Language|first-order language]]  defines a specific meaning or set of interpretations for a first-order language.

>[!summary] Definition
>Generally, a model consists of the following:
>1. Domain: a non-empty set of objects $M$
>2. Interpretation of constant symbols: for each constant $c \in \mathscr{L}$, an object $c^{\mathfrak{M}} \in M$
>3. Interpretation of predicate symbols: for each $n$-ary predicate symbol $R \in \mathscr{L}$, an $n$-ary relation $R^{\mathfrak{M}} \subseteq M^{n}$
>4. Interpretation of function symbols: for each $n$-ary function symbol $f \in \mathscr{L}$, an $n$-ary function $f^{\mathfrak{M}}:M^{n} \to M$