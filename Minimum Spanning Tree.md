---
aliases: [MST]
---
#programming #data_structures #graph_theory #mathematics 

An instance of a [[Tree (Data Structure)|tree]] that has a minimum weight.

>[!note] Formally
>A subset of the [[Graph (Data Structure)|graph's]] edges that connect all [[Vertex|vertices]] in the graph together with the minimum sum of edge weights.
>>[!warning]
>>The graph must be weighted and connected. A connected graph contains a **path** (not an [[Edge (Data Structure)|edge]]) between every pair of vertices

## Kruskal's MST Algorithm
*Repeat until all nodes are connected*
1. Pick the [[Edge (Data Structure)|edge]] with the smallest weight remaining such that the two [[Vertex|nodes]] it connects are not already connected
2. Add the edge to the set of MST edges

Space Complexity: O(V + E)
[[Runtime Complexity|Time complexity]]: O(E log E) w/ efficient vertexSet implementation, O(E * V) without efficient vertexSet