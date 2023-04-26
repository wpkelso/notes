#compilers #computer_architecture #computer_hardware 

**Problem:** [[Static Single-Assignment|SSA form]] assumes an infinite number of virtual registers, but actual [[Computer Architecture|architectures]] have a limited number of [[Register|registers]] (For example, the [[LC-3 Architecture]] has only 4 general-use registers). Therefore, not all program values can be kept within a register, and we need a **solution** that maps *virtual* registers to *physical* registers.

## [[Hueristic]]