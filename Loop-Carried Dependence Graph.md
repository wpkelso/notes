---
tags: [graph_theory, parallel_computing, programming]
---

# Loop-Carried Dependence Graph

A way of displaying [[Data Dependence|dependencies]] across loop iterations. In an LDG, the nodes correspond to a point in the iteration space, and directed edges show the direction of the dependence. LDGs do *not* show loop-independent dependencies, only [[Loop-Carried Dependency|loop-carried dependencies]].