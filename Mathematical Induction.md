---
tags:
  - mathematics
  - discrete_mathematics
created: 2023-09-12T13:58
updated: 2023-09-12T14:18
---

# Mathematical Induction

Mathematical induction is a [[Mathematical Proof|proof]] strategy used in situations where it is easy to go from one case of the problem to the next.

## Formal Structure

Like any formal proof, proofs by induction follow a certain structure.

>[!summary] Structure
>“Let $P(n)$ be the statement $\dots$”. Then to prove for $P(n)$ for all $n \geq 0$, prove the following:
>1. Base case: Prove $P_{0}$
>2. Inductive Case: Prove that for any $k \geq 0$ if $P(k)$ is true, then $P(k+1)$ is true as well. (As this is an inductive hypothesis, assume $P(k)$ is true).
>Assuming both parts are successful, the conclusion can be “Therefore by the principle of mathematical induction, the statement $P(n)$ is true for all $n\geq 0$.”
*It should be noted that 0 can be replaced with another number should the bounds of the statement be nonzero.*