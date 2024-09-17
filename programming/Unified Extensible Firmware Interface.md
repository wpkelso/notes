---
aliases:
  - UEFI
  - EFI
  - Extensible Firmware Interface
tags:
  - computer_architecture
  - programming
created: 2023-11-05T22:50
updated: 2024-09-16T17:37
---

# Unified Extensible Firmware Interface

> [!summary]
> Unified Extensible Firmware Interface, or UEFI for short, is a specification developed to replace [[Basic Input Output System|BIOS]] as the architecture defining platform firmware and it’s interface for interacting with the [[Operating System|operating system]].

The UEFI Forum was established in 2005, following the release of the last specification of EFI (an in-between stage developed by Intel), which was subsequently donated as a contribution to the UEFI Forum.

## Terminology

The terminology used to refer to UEFI varies widely between organizations:

- Major computer systems supply chain industry players refer to their bootstrap firmware as BIOS
- Microsoft uses UEFI
- Apple uses EFI, execept in security documentation where they use UEFI

Additonally:

- Firmware providing [[Basic Input Output System|BIOS]] functionality is typically called “Legacy BIOS”
- Platform Initialization (PI) and UEFI compatible firmware implementations are sometimes called UEFI BIOS, or just UEFI

## Goals

Initially, EFI was intended to:

- Replace assembly with a high level language
- Grow with new innovations in computing (i.e. 64-bit processors)
- Provide a more stable, open-source specification for a core component of modern computing

UEFI has now grown to encompass five main goals:

1. Provide a coherent, scalable platform environment that can be consumed by the OS and will work for a wide range of designs
2. Abstract the OS from the firmware, providing stable and minimal interfaces for OSes to work with
3. “Reasonable” devices abstraction, that enable support for a wide range of underlying hardware, free of legacy interfaces
4. Abstraction of Option [[Read-Only Memory|ROMs]] from the firmware, allowing clear separation between the two
5. Create an architecturally shareable system partition, allowing platform feature expansion through clearly defined methods by which additional applications can use mass storage