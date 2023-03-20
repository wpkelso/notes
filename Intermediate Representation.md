#compilers 
The IR is an assembly or assembly-type language designed to generically represent a wide variety of [[Instruction Set Architecture|ISAs]] agnostically.

*Ex.* LLVM IR

The IR is critical for fulfilling general compilation goals such as ease of analysis, fast compile time, producing good quality code, and being debuggable.

## IR Taxonomy
- Structural representation
	- [[Graphical Intermediate Representation]]
	- [[Linear Intermediate Representation]]
	- [[Hybrid Intermediate Representation]]
![[Pasted image 20230213222958.png]]
- Level of Abstraction : refers to the spectrum of IR possibilities between language and machine code.
- Expressiveness: the ability of the IR to accommodate all the facts the compiler needs to record. **The IR is the only thing guaranteed to survive between one compilation stage to the next,** so if information is not encoded in the IR it might as well not exist.

## Generating IR
- As each rule is matched, perform an action that builds the necessary IR
- Compilers will generally provide a set of functions that help build the intermediate representation as IR can be complex, so this reduces the likelihood of building incorrect IR, and saves the developers the effort of recreating such code on their own

## Representing Information
As IR is just Control Flow + Data Flow, its useful to have methods for representing both of these types of information. Control flow information is represented with the [[Control Flow Graph|control flow graph]]. Data flow information, or data dependencies, are widely represented in [[Static Single-Assignment|SSA form]].