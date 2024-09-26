---
aliases:
  - HOB
created: 2024-09-26T12:38
updated: 2024-09-26T12:38
---

# Hand-Off Block (HOB)

> [!summary]
> Binary data structures used to pass information between Pre-EFI Initialization and further UEFI boot phases.
> They contain information on various I/O media, such as system memory, (MM)I/O resources, and firmware devices and volumes.
> Additionally, HOBs contain information on the boot-path

At runtime, HOBs are stacked together to enable flexible amounts of information to be passed.
The HOB list is built in PEI and DXE phases, or the “limited memory phase” and the “main initialization phase” respectively.
