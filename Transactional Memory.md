---
tags: computer_architecture, parallel_computing
created: 2023-11-13T13:37
updated: 2023-11-13T14:04
---

# Transactional Memory

Builds upon two main elements:

- Conflict detection
- Data versioning

> [!info] Transaction
> A set of instructions that execute fully or all get discarded without being visible to other threads, _unless all instructions complete successfully_. these concepts are referred to as **atomicity** and **isolation**.
> In the world of databases, the qualities of a transaction is expanded to included **durability**, where the updates of a successful transaction are retained even in catastrophic events; and **consistency**, where a transaction takes the system from a consistent state to another.

## Data Versioning 

### Eager Versioning

Everything is updated in place in memory during the transaction. However, if it fails, there needs to be some rollback mechanism to recover the previous value of the memory location.

This makes it faster to commit data in the case where there is no conflict, but aborting a transaction is more complicated and slower.

### Lazy Versioning

Buffer changes to memory, then only update at the point of commit. Opposite to eager versioning, commits are slower, as they get buffered; however, aborting a transaction is much faster as no recovery of memory needs to be performed.

## Conflict Detection

A conflict occurs in transactional memory when there is an overlap between the read sets and/or write sets of two transactions (W-W, R-W for the same address).