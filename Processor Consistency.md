---
tags: parallel_computing, computer_architecture
---

# Processor Consistency

Processor consistency is a [[Memory Consistency|memory consistency]] architecture intended to decrease the amount of time a [[Computer Processor|processor]] needs to wait  to execute instructions by relaxing the ordering between [[Memory Instructions|stores and loads]]. 

## Local Write Buffer

Consistency is achieved by allowing local write buffers that allow stores to be buffered, and not written to [[Cache|cache]] until later. This can create a situation where younger loads can appear globally before older stores. The local write buffer is a FIFO buffer, meaning that stores must still be committed in order, but interactions with loads can appear to happen out of order.