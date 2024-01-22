---
tags: programming, embedded_systems
created: 2024-01-21T21:45
updated: 2024-01-21T21:46
---

# Lifetime

The period of time from the allocation of a [[Variable|variable]] in [[Memory|memory]], until it is deallocated. Generally, three types of allocation are considered, so three general lifetimes can be associated with them, as follows:

1. Statically allocated variables: Exist from program start to end, with each variable having a fixed location so space is _not_ reused
2. Automatically allocated variables: Exist from [[Function|function]] start to end, each variable does not have a fixed location, so space can be reused
3. Dynamically allocated variables: Exists on the [[Heap|heap]] from explicit allocation to explicit deallocation. Each variable does not have a fixed location, so space can be reused
