---
tags: [parallel_computing, computer_architecture]
---

# MOESI Protocol

Further extending [[MESI Protocol|MESI]] and [[MSI Protocol|MSI]], MOESI protocol adds the “Owner” state. The “O” state represents a copy more recent than in main [[Memory Block|memory]], but where copies may also be present in other cores.

Requesting Core:
![[Pasted image 20231001164129.png]]

Receiving Core:
![[Pasted image 20231001164139.png]]