---
tags: computer_architecture, parallel_computing
---

# Weak Ordering

[[Memory Consistency|Memory consistency]] architecture based on the assumption that programmers tell the hardware where the program needs to be synchronized. The rest of the instructions get ordered with respect to these synchronization points. These larger blocks of instructions can be reordered internally however they need to be, but instructions cannot be reordered across blocks.