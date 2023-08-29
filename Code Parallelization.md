---
tags:[computer_architecture, programming]
---
# Code Parallelization

Typically, there are 4 major steps to any [[Parallelization|parallelization]] scheme:

1. Decomposition: dividing the program into parallel tasks
2. Assignment: assigning tasks to the parallel processes
3. Communication: sync between the different processes
4. Mapping: mapping processes into hardware processing elements

## Methodologies for Parallelizing Code

### Distributed Loop

Distributed is the scheme used when a loop iteration contains [[Loop-Carried Dependency|loop-carried dependencies]], as well as other [[Instruction|instructions]] that do not carry a dependence on other iterations.

### DOALL

DOALL is the scheme used when every iteration in a loop is independent for all others. This creates a situation where theoretically each thread can take as little as one iteration to execute in parallel.

### DOACROSS

DOACROSS is the scheme used when an iteration can be divided into a parallel and a dependency part. Each iteration directly notifies the iteration depending on it once the result is ready.

### DOPIPE

DOPIPE is a scheme in which a loop is divided into two parts/threads: a producer and a consumer. This requires a lot of communication.