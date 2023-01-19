#compilers 
## Key Goals
- **Produce very high quality code:** Compilers contain a large set of optimizations and analyses that are meant to make the code faster and/or smaller
	- *Ex:* Avoid accessing memory, redundancy elimination, optimize loops, using resource effectively, etc.
- **Complete its task in a reasonable amount of time:** compiler needs to be fast, but the generated code needs to be optimal (which will take longer to figure out)
	- Many compilers problems are NP-Complete. This means that we have to use heuristics, and compilers tend to adopt algorithms that are nor worse than O($n^3$)
	- *This means that compilers can't necessarily create **optimal** code, only **optimized** code*
- Bug-free and extensible: compilers must correct output on all possible programs
	- Even subtle or minor bugs in the implementation of such algorithms can have dire consequences
	- **Strategies:** Divide compiler into passes that conform to a well defined set of inputs and outputs, build excessive assertions and checks into the standard operation of the software, log intermediate forms of the program to help track down bus, extensive testing, and thoroughly documented code
### Other Goals
*(Less important but still good to keep in mind)*
- Feedback to the user
- Source-level Debugging support

## Typical Parts of a Compiler
Source Files -> [[Compiler Front End|Front End]] -> Optimizer -> Machine Code Generator -> Object code or Executable

*In reality, there will be support for multiple front end and multiple machine code generators, so there will be [[Intermediate Representation|intermediate representations]] that the optimizer will only work on*