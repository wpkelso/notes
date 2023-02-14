#data_structures #ECE309 #graph_theory #programming 

>[!note] Definition
>Orders the nodes in a [[Directed Acyclic Graph|DAG]] such that the source of an [[Edge|edge]] occurs before the destination of the edge

## Implementations
- Approach 1:
	1. Keep track of the incoming edges to a node
	2. Once all of a node's incoming edges are scheduled, schedule it
```psuedocode
GraphTopologicalSort(graph) {
	resultList = empty list of vertices
	noIncoming = list of all vertices with no incoming edges
	remainingEdges = list of all edges in the graph

	while (noIncoming is not empty) {
		currentV = remove any vertex from noIncoming
		Add currentV to resultList
		outgoingEdges = remove currentV's outoing edges from remainingEdges
		for each edge currentE in outgoingEdges {
			inCount = GraphGetIncomingEdgeCount(remainingEdges, currentE->toVertex)
			if (inCount == 0)
				Add currentE->toVertex to noIncoming
		}
	}
	return resultList
}
```

- Approach 2:
	1. Reverse post-order (visiting the [[Vertex|node]] *after* recursively visiting it's adjacent nodes) [[Depth First Search|DFS]] traversal
```psuedocode
TopologicalSort(graph) {
	list = find all nodes in graph with no incoming edges
	sortedList = {}
	for each node in list {
		RecursiveDFS(node)
	}
}
RecursiveDFS(node) {
	if ( node is not in visitedSet ) {
		Add node to visitedSet;
		for each vertex adkV adjacent to node {
			RecursiveDFS(adjV);
		}
		insert node at head of sortedList // reverse the list as we go
	}
}
```