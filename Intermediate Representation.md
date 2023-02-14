#compilers 
The IR is an assembly or assembly-type language designed to generically represent a wide variety of ISAs agnostically.

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