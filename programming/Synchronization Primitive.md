---
tags: parallel_computing, computer_architecture, programming, hardware
created: 2023-11-30T16:22
updated: 2023-11-30T16:47
---

# Synchronization Primitive

A synchronization primitive is—as the name would suggest, are structures that are used to ensure synchronization between processes in [[Parallelization|parallelization]].

General practice is to implement the lowest level primitives in hardware as [[Instruction|atomic instructions]], then implement all other primitives on top of that in software.

## Software

In software, common primitives are [[Lock|locks]], [[Barrier|barriers]], and [[Point-to-Point Synchronizations|point-to-point synchronizations]] (i.e. signal-wait pairs).

The [[Code Parallelization#DOALL|DOALL code parallelization]] method and applications that use linked [[Data Structure|data structures]] rely heavily on the aforementioned locks and barriers. On the other hand, point-to-point is essential for [[Pipelining|pipelined]] parallelism schemes such as [[Code Parallelization#DOACROSS|DOACROSS]].
