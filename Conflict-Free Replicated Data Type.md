---
aliases:
  - CRDT
created: 2024-10-04T15:17
updated: 2024-10-04T22:01
---

# Conflict-Free Replicated Data Type

> [!summary]
> A [[Data Structure|data structure]] that replicates across multiple computers in a network, with three key features:
>
> 1.  Any replica can be updated independently, concurrently, and without coordinating with other replicas
> 2.  An [[Algorithm|algorithm]] that automatically resolves an inconsistences that might occur.
> 3.  Replicas may have a different state at any particular point in time, they are guaranteed to eventually converge

CRDTs are a practical use of [[Optimistic Replication]].

## Operation-based CRDTs

_a.k.a. Commutative replicated data types_

State is propagated via the transmission of only update operations. All replicas receive updates and then apply them locally. These operations are commutative but are not necessarily idempotent. As a consequence operations can arrive in any order, _but must all arrive._

## State-based CRDTs

_a.k.a. Convergent replicated data types_

State is propagated by sending the full local state to all replicas, which is then merged by a function that must be commutative, associative, and idempotent. 