---
created: 2024-10-21T13:55
updated: 2024-10-21T13:55
---

# Boot Device Selection

>[!summary]
>The final interface between the firmware and the OS, as well as the final stage in the [[Platform Initialization]] process. 
>BDS facilitates selection of and initialization of the boot process for the OS, or some other transient boot application.

## Issues Responsibility

The presence of this stage can create some confusion for some in some scenarios; many operating systems integrate the OS loader, so the presence of a discrete bootloader such as GRUB may cause issues.