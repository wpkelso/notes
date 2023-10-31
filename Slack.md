---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#compilers 
A [[Heuristic|heuristic]] calculating the difference between the earliest time an operation can execute ([[Data Dependence Depth|Depth]]) and the latest time an operation can execute ([[Data Dependence Height|Height]]) without slowing down the program, assuming infinite resources. Slack is generally considered the best heuristic, but is not infallible.

## Calculation
1. Find height for operation
2. Find depth for operation
3. Height' = Schedule height - Height + 1
4. Slack = Height’ - Depth
*The schedule height is the largest height in the schedule*