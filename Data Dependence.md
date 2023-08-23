---
tags:[computer_architecture]
---
# Types of Dependencies
## True Dependency
ISNT2 reads a [[Variable|variable]]/location written earlier by INST1.

## Anti-Dependency 
INST2 writes a variable/location read previously by INST1

## Output Dependency
INST1 and INST2 write to the same variable/location

## Input Dependency
INST1 and INST2 read from the same variable/location

>[!important] 
>Anti & Output dependencies are also called **Name dependencies**