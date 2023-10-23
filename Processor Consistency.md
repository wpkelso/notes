---
tags: [parallel_computing, computer_architecture ]
---

# Processor Consistency

Processor consistency is a memory consistency architecture intended to decrease the amount of time a [[Computer Processor|processor]] needs to wait  to execute instructions by relaxing the ordering between [[Memory Instructions|stores and loads]]. It does this by allowing local write buffers that allow stores to be buffered, and not written to [[Cache|cache]] until later. This can create a situation where younger loads can appear globally before older stores.