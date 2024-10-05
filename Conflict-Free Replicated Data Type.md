---
aliases:
  - CRDT
created: 2024-10-04T15:17
updated: 2024-10-04T18:40
---

# Conflict-Free Replicated Data Type

> [!summary]
> A [[Data Structure|data structure]] that replicates across multiple computers in a network, with three key features:
>
> 1.  Any replica can be updated independently, concurrently, and without coordinating with other replicas
> 2.  An [[Algorithm|algorithm]] that automatically resolves an inconsistences that might occur.
> 3.  Replicas may have a different state at any particular point in time, they are guaranteed to eventually converge

## Operation-based CRDTs

_a.k.a. Commutative replicated data types_

## State-based CRDTs

_a.k.a. Convergent replicated data types_
