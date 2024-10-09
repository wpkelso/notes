---
created: 2024-10-09T15:18
updated: 2024-10-09T15:37
---

# Boot Manager

> [!summary]
> Program within [[Unified Extensible Firmware Interface|UEFI]] responsible for loading various types of specified applications, and provides required configuration

## Types of Recognized UEFI Binaries

| Type                                                        | Description                                                                                                                                                                                                                                                                                                      |     |
| ----------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --- |
| Images                                                      | Files containing executable code, using a subset of the PE32+ image format. Differentiated via a machine paramter, describing the processor architecture of the executable; and subsytem describing if the executable is an application, [[Boot Service\|boot service]], or [[Runtime Service\|runtime service]] |     |
| Applications                                                | Loaded by the bootloader or other UEFI applications and can perform boot exit services                                                                                                                                                                                                                           |     |
| OS Loaders                                                  | Special type of application that takes over platform control and passes it to the [[Operating System\|OS]]                                                                                                                                                                                                       |     |
| [[Unified Extensible Firmware Interface#Services\|Drivers]] | Two types: boot services and runtime service                                                                                                                                                                                                                                                                     |     |
