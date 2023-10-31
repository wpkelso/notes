---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#computer_architecture 

## Pipelined Processors
A [[Cache]] miss will stall the [[Datapath Design|MEM stage]]. As instructions proceed in order, previous stages will be stalled as well so the whole pipeline becomes stalled.

## Out of Order Processors 
Multiple instructions can issue, read operands, execute, and commit in parallel so memory latencies are partially hidden by overlapped instruction execution. Therefore the miss penalty is the non-overlapped miss latency. Thus the we can define 
$$\text{Memory stall cycles/instruction}=\text{Misses/instruction}*(\text{total miss latency }-\text{ overlapped miss latency})$$

### Defining Miss Latency 
There is no single answer for how to define miss latency. It could be defined from when the instruction is queued in the instruction queue, when the address is generated, or when the instruction is sent to the memory system.