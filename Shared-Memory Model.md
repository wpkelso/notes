---
tags: parallel_computing, computer_architecture
created: 2023-09-08T14:31
updated: 2023-11-30T16:17
---

# Shared-Memory Model

A model of [[Parallel Computing]] where all parallel tasks run within the same _virtual address space_. These tasks within the same address space are called **threads**, while the private address space is called a **process**. As such, all memory can be seen by every task.

> [!note] Definition
> **Process:** A private address space.

> [!note] Definition
> **Thread:** A task within a shared address space.
