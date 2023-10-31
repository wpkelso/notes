---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#computer_architecture #programming 
Forms the [[computer architecture]], along with the [[Microprocessor Architecture]]

Includes:
- Organization of programmable storage (registers, memory)
- [[Data Type]]: encodings & representations
- Instruction set & formatting
- [[Addressing Modes|Modes of addressing]] and accessing data & instructions
- Exception conditions (*Ex.* Division by zero)

## Programmer's Interface
ISA designers need to answer the question, "What does the programmer need?" Instruction set information should include the available operations, the branching behavior, and valid instruction sequences. The [[Register|register]] part of the ISA should include the number, sizes, and data types of the available registers.

However, the implementation of the ISA falls to the [[Microprocessor Architecture]].

### Assembly Characteristics
#### Instructions
Primitive operations:
- [[Arithmetic Instructions]] perform arithmetic functions on register or memory data (ADD, SUB)
- [[Memory Instructions]] transfer data between memory and register (LOAD from memory to register, STORE register data into memory)
- [[Control Flow Instructions]]
	- Conditional branches
	- Unconditional jumps to/from procedures
### Data Types
Minimal Data types:
- Integer data of 1, 2 or 4 bytes
- Floating point data of 4, 8, or 10 bytes
- No aggregate types such as arrays or structures (purely contiguously allocated bytes in memory)
#### Addressing Modes
Many different types available in [[Complex Instruction Set Computers|CISC]] architectures
*Ex.*
- Register (ADD R4, R3)
- Immediate (ADD R4, #3)
- Displacement (ADD R4, 100(R1)); local variables & register indirect

## Formats
**R-Format:** register to register format
**I-Format:** immediate format
**J-Format:** jump/branch format