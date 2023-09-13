---
tags: [computer_architecture, parallel_computing, electronics]
---

# Cache Coherency

In [[Parallel Computing|parallel computing architectures]], each [[Computer Processor|core]] in the system will have it’s own [[Cache|cache]] in between it and the main memory. This creates an issue during [[Parallelization|parallelization]], where a cache block might contain data that has been modified somewhere else in the system, such as in other caches or in the [[Computer Memory|main memory]]. This is generally implemented in modern processors through hardware.