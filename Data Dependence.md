---
tags:[computer_architecture]
---
# Types of Dependencies
## True Dependency
ISNT2 reads a [[Variable|variable]]/location written earlier by INST1. This creates a situation where instructions must be evaluated in order.

## Anti-Dependency 
INST2 writes a variable/location read previously by INST1. This can be solved through *privatization* to still allow reordering

## Output Dependency
INST1 and INST2 write to the same variable/location.

>[!important] 
>Anti & Output dependencies are also called **Name dependencies**

## Input Dependency
INST1 and INST2 read from the same variable/location
