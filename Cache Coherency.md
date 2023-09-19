---
tags: [computer_architecture, parallel_computing, electronics]
---

# Cache Coherency

In [[Parallel Computing|parallel computing architectures]], each [[Computer Processor|core]] in the system will have it’s own [[Cache|cache]] in between it and the main memory. This creates an issue during [[Parallelization|parallelization]], where a cache block might contain data that has been modified somewhere else in the system, such as in other caches or in the [[Computer Memory|main memory]]. This is generally implemented in modern processors through hardware.

## Protocols

### Update-Based

The general idea with an update based protocol is that every time a cache block is update, all potential copies in the system are updated. This is faster for producer/consumer systems where one thread is constantly using the product of another. However, this can get expensive in bandwidth.

### Invalidation-based Coherence

Each time you update a local copy in a cache, invalidate all other possible copies in other caches. This causes caches to miss and explicitly request for a new copy. This creates a situation where subsequent write hits are local, so there is no extra bus traffic. However, this is complicated and poor for a produce-consumer pattern as it creates many misses at the consumer side.

>[!info] 
>Most modern processors use invalidation-based coherence rather than update-based.

#### MSI Protocol

The MSI protocol is an example of an invalidation-based protocol. In it, any time a cache block must be in one of the following states:
- **M**odified
- **S**hared
- **I**nvalid
