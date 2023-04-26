#computer_science #hueristics #mathematics 

Based on the classic problem of coloring countries on a map a different color, this [[Hueristic|hueristic]] models the countries as [[Vertex|nodes]] on the [[Graph|graph]], with [[Edge|edges]] representing a shared border. The goal, of course, is to give countries with a shared border a different color.

## Problems and Reasons for Existing
- Coloring a graph with $k$ colors where $k\geq 3$ is [[Algorithm#NP-Completeness|NP-complete]] and thus a hueristic **must** be used.

## [[Algorithm]]
**Goal:** color the graph with at most $k$ colors
**Observation:** (Made by Chaitan in 1981) If $G'=G-\{x\}$ can be colored in $k-1$ colors, then $G$ can be colored in $k$ colors

1. Repetedly delete nodes with degree $<k$
2. Push deleted nodes onto a stack (observe that each deletion creates new nodes with degree$<k$)
3. Continue until only 1 node remains
4. Starting with the last node, assign a color
5. Pop nodes from the stack and assign a color