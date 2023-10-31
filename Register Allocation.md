---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#compilers #computer_architecture #computer_hardware 

**Problem:** [[Static Single-Assignment|SSA form]] assumes an infinite number of virtual registers, but actual [[Computer Architecture|architectures]] have a limited number of [[Register|registers]] (For example, the [[LC-3 Architecture]] has only 4 general-use registers). Therefore, not all program values can be kept within a register, and we need a **solution** that maps *virtual* registers to *physical* registers.

## [[Hueristic]] Approach
Considering the [[Liveness Analysis#Register Live Range|live range of a register]], two live ranges that overlap are said to **interfere**, and must be assigned to different registers. These relationships can be represented through an [[Interference Graph|interference graph]]. Assignment is then done with [[Graph Coloring Hueristic|graph coloring]]. 
>In the specific case of register allocation, if a system doesn’t have enough physical registers to color the graph, some registers must be [[Register Spill Hueristic|spilled to memory]] even if an optimal [[Algorithm|algorithm]] would succeed.