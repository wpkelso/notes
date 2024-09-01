---
alias:
  - BIOS
created: 2024-08-29T16:12
updated: 2024-08-29T16:12
---

# Basic Input/Output System

>[!summary] 
>x86 Assembly-based boot firmware implementation that provided basic initialization and configuration services for CPUs


## History

First developed in 1975 by Gary Kildall, the BIOS was the first host CPU boot [[Firmware]] implementation, and was in use for thirty years before being succeeded by [[Unified Extensible Firmware Interface|UEFI]].
By 1990, it was considered mostly obsolete, and was hard to adapt to new hardware---not to mention that it was closed source with a proprietary licence.

## Implementation
BIOS was written in pure [[Intel x86|x86]] assembly, and provided hardware initialization, configuration utilities, and runtime services.
