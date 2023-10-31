---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#computer_hardware #computer_architecture 

System using multiple levels of [[Cache|caches]] to try and optimize the cache more. Generally, the first level is quite small, allowing for a reduced hit time, while the second level is larger, creating a decrease in the miss-rate. *More levels are possible beyond the two mentioned here.*

![[Pasted image 20230426184332.png]]

## Effect on Average Memory Access Time
$$\text{Avg memory access time}=\text{Hit time}_{L1}+\text{Miss rate}_{L1}*(\text{Hit time}_{L2}+\text{Miss rate}_{L2})$$
The miss rate of $L\{n\}$is equal to the avg memory access time of $L\{n+1\}$.

The local miss rate is equal to cache misses/cache accesses, while the global miss rate is equal to cache misses/memory accesses. As such, the global miss rate for $L\{n\}$ is equal to the local miss rate for $L\{n\} * L\{n-1\}*\dots*L\{1\}$

## Multilevel Inclusion
*L1 data is **always** present in the L2 cache*
This has the advantage of consitency between caches and I/O or in a multicore setting only the L2 cache needs to be checked. However, a mismatch in block size between L1 and L2 maens that eviction on L2 will invalidate all corresponding L1 blocks, increasing the L1 miss rate.

## Multilevel Exclusion
*L1 data is **never** present in the L2 cache*
When a cache miss happens on L1 it causes a swap in blocks between L1 and L2. This has the advantage of avoiding data redundancy in two cases, but wastes L2 space.