---
aliases:
  - DXE
tags:
  - programming
  - computer_architecture
  - uefi
created: 2024-09-19T13:28
updated: 2024-10-21T13:45
---

# Driver Execution Environment

> [!summary]
> The final stage of [[Platform Initialization]], the DXE is where device initialization occurs.
> It provides a common interface for all drivers, and a full execution environment with access to a DRAM address space and other services.

## Services

Access to the full DRAM address range means that there is a much larger variety of services within DXE. These include

- Task priority management
- Memory allocation, retrieval of the memory map
- Events & timers
- Protocol management services
- Image services for loading PE/COFF executable images
- Driver management services for registering and un-registering drivers
