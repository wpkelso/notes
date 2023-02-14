---
aliases: ["Syntax Directed Analysis"]
---
#compilers 
To figure out if the program has valid meaning:
1. Associate [[Semantic Attributes|semantic attributes]] with productions in a [[Grammar|grammar]]
	1. These may be actions
2. Test/apply attributes while translating the input
	1. Part of the action associated with a production is is testing of attributes
3. If no attributes are violated, the program is valid (but not necessarily bug-free).