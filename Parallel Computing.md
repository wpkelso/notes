---
tags: [computer_architecture, programming]
---
# Parallel Computing

A style of computing where multiple processing elements communicate and work together to solve a problem through [[Parallelization|parallelization]].

## Components

1. **Processing Element:** logic that can execute instructions
2. **Communication between processing elements**:
	1. [[Shared-Memory Model|Shared-memory]]: implicit sharing through read/write operations to shared memory
	2. [[Message-Passing Model|Message-passing]]: explicit sharing through send/receive messages between tasks
	3. Hybrid model: combines the two models above

| Aspects                   | Shared Memory        | Message Passing         |
| ------------------------- | -------------------- | ----------------------- |
| Communication             | implicit (via LD/ST) | explicit messages       |
| Synchronization           | explicit             | implicit (via messages) |
| Hardware Support          | typically required   | none                    |
| Development effort        | lower                | higher                  |
| Tuning effort             | higher               | lower                   |
| Communication Granularity | finer                | coarser                 | 

