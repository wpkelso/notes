---
tags:
  - UEFI/BIOS
  - Programming
  - Computers
  - Firmware
created: 2024-10-10T12:37
updated: 2024-10-10T13:23
---

# Platform Initialization

## Phases

There are four stages to platform initialization:

1. Security (SEC)
2. Pre-EFI Initialization (PEI)
3. Driver Execution Environment (DXE)
4. Boot Device Selection (BDS)

### Security

Described in Chapter 13 of the Platform Initialization specification.
This phase starts at the reset vector, so it includes the most basic initialization tasks (entering protected mode, loading microcode, etc.)
SEC serves as the “root of trust” for UEFI, as it is what is able to authenticate the PEI foundation.

The SEC phase is expected to pass the following information to PEI foundation:

- State of the platform
- Location and size of the Boot Firmware Volume (BFV)
- Location and size of of temporary RAM
- Location and size of the [[Stack|stack]]
- Optionally, one or more [[Hand-Off Block|HOBs]] via [[Unified Extensible Firmware Interface#Protocols|UEFI protocols]]

### Pre-EFI Initialization

The primary subject of the PI specification, the PEI phase will often contain proprietary information and code.
PEI has four primary goals:

1. Maintain chain of trust consistency
2. Perform early initialization
3. DRAM initialization
4. Prepare HOB data for DXE and pass control to it

It’s structure closely resembles that of DXE, but PEI must cope with more limited access to memory resources.

Six elements make up PEI:

1. PEI Foundation: general code managing PEI execution and transition to DXE
2. PEI Modules (PEIMs) → single purpose, interchangeable pieces of initialization code
3. PEIM-to-PEIM interfaces ([[Unified Extensible Firmware Interface#Protocols| PPIs]]) → provide communication between modules
4. PEI Dispatcher → a state machine implemented in PEI foundation iterating over available PEIMs and running them
5. PEI Services → set of core operations used in PEIMs
6. Dependency Expressions (DEPEX) → each PEIM has a set of PPI GUIDs that must be loaded before itself
