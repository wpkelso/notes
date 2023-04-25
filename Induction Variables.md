#compilers #programming 
An **induction variable** is a variable that gets increased or decreased by a fixed amount on every iteration of a loop, or that is a linear function of another induction variable. [[Induction Variable Analysis]] is used to find these induction variables, and [[Strength Reduction]] is used to simplify them.

A *basic* induction variable will have a closed update chain in the [[Static Single-Assignment|SSA]] graph. This has a couple of important properties:
- The update and the [[Phi-Node|phi-node]] must create a closed cycle where the phi-node is in the loop header
- Only add and subtract operations with a constant step operand are allowed
- The increment operation must dominate the back edge

A *related* induction variable will show a modification to the original induction variable. These could take the form of any add, sub, multiply, 