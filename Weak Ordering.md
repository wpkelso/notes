---
tags: computer_architecture, parallel_computing
created: 2023-10-23T14:17
updated: 2023-10-23T14:21
---

# Weak Ordering

[[Memory Consistency|Memory consistency]] architecture based on the assumption that programmers tell the hardware where the program needs to be synchronized. The rest of the instructions get ordered with respect to these synchronization points. These larger blocks of instructions can be reordered internally however they need to be, but instructions cannot be reordered across blocks.