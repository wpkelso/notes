#embedded_systems #ECE460 

>GPIOx_PDOR (Port Data Output Register)
>GPIOx_PSOR ()
>GPIOx_PCOR ()
>GPIOx_PTOR ()
>GPIOx_PTOR ()
>GPIOx_PDDR (Data Direction Register) used to control whether the GPIO is configured as a 

### Clocking
By default, clocks aren't enabled for the port modules to save power. The System Integration Module (SIM) is used to control clock enablement to port modules (Specifically SIM_SCGC5).

**Writing to an unclocked module triggers a hardware fault**

### Accessing Peripheral Control Bits
- Software methods to organize and access groups of control registers at specific addresses
	- C language **struct** data types
	- [[CMSIS]]-CORE Device PAL support
- Software methods to access to specific bits within a control register

### PORT and GPIO Control Registers in Memory
Memory is divided into general spaces: code, SRAM, Peripheral, external RAM, External device, Private Peripheral Bus, and System. Within those spaces, specific ports and pins have blocks of memory assigned to each