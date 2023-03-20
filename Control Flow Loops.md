#compilers #automata 
## Natural Loops
A loop in a well-formed program has the following properties:
- A definite entrance or header basic block
- A definite set of [[Back Edge|back edges]]
- The body of the loop is all the [[Vertex|nodes]] on a path from A to B without returning to A
>[!note] 
>Not all [[Cycle|cycles]] in a [[Control Flow Graph|CFG]] are loops
## Inner Loops
Defined as when a loop only has one [[Back Edge|back edge]], or if all the back edges have the same header. In other words, no blocks constitute another loop.