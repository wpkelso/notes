---
tags:
  - parallel_computing
  - computer_architecture
created: 2023-10-01T16:38
updated: 2023-10-01T16:41
---

# MOESI Protocol

Further extending [[MESI Protocol|MESI]] and [[MSI Protocol|MSI]], MOESI protocol adds the “Owner” state. The “O” state represents a copy more recent than in main [[Memory Block|memory]], but where copies may also be present in other cores.

Requesting Core:
![[Pasted image 20231001164129.png]]

Receiving Core:
![[Pasted image 20231001164139.png]]