---
tags:
  - parallel_computing
  - computer_architecture
created: 2023-10-01T16:22
updated: 2023-10-01T16:34
---

# MESI Protocol

The MESI protocol is an extension of the [[MSI Protocol|MSI protocol]],  adding the “Exclusive” state. This state represents an item that is *only* present in the current cache, and that is *clean*. From the “E” state, the item may go to the “S” or the “M” state at any time.

![[Pasted image 20231001163419.png]]

![[Pasted image 20231001163427.png]]