#computer_architecture 
Primary control unit within a computer. Performs all [[Instruction Set Architecture|instructions]], reads and writes to memory, etc.

### Data Path
A simple processor data path will have a [[Register File|register file]] to store data, memory (DRAM & disk) and a primary path of instruction fetch -> decode -> execute -> memory -> write back.

## Performance Evaluation
The measure of performance used for processors is how long a tasks takes, as well as the number of instructions processed per unit time.

### [[Amdhal's Law]]
$$S_{\text{latency}}(s)=\frac{1}{(1-p)+\frac{p}{s}}$$
### Iron Law
$$\text{CPU time} = \text{(instruction count} * \text{clock cycle per instruction)} * \text{clock cycle time}$$

CPI = average number of clock cycles/instruction
IPC = 1/CPI = average number of instructions/clock cycles

### What affects performance?
- Instruction Count
	- Software algorithm, compiler, [[Reduced Instruction-Set Computers|RISC]] vs [[Complex Instruction Set Computers|CISC]] architecture
- Clock-cycle-per instruction
	- Hardware (pipe-lining, branch prediction, caches, etc.), compiler
- Clock Cycle Time
	- Technology Scaling
	- Simple ISA -> Simple Microarchitecture
	- Deeper pipelining