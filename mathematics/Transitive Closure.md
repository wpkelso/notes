---
tags:
  - discrete_mathematics
  - graph_theory
  - programming
  - mathematics
  - set_theory
created: 2023-10-17T17:01
updated: 2023-10-17T17:19
---

# Transitive Closure

The transitive closure of a set is defined as the smallest relation on a set $X$ that contains a relation $R$ and is [[Transitivity|transitive]]. Commonly, transitive closure is used to solve reachability questions (i.e. can one reach a node $x$ starting at node $y$).

Below is an example of a an application of transitive closure on a [[Directed Acyclic Graph|DAG]].
![[Pasted image 20231017170838.png]]

>[!Help] 
>For further reading, see [this](https://en.wikipedia.org/wiki/Transitive_closure) link

## Matrix Representation

Transitive closure can be seen easily when a reachability [[Matrix|matrix]] is created, defined as a $n \times n$ matrix where a node that is reachable from another is shown with a 1, and a node that is unreachable is shown with a 0.