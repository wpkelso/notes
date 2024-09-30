---
created: 2023-09-08T14:31
updated: 2024-09-30T11:51
---
#computer_hardware #computer_architecture 

## Basic [[Cache]]Optimizations
1. **Larger block size:** this will reduce the miss rate (compulsory misses), but too large of a block size may increase the miss penalty
2. **Larger cache:** this will reduce the miss rate (capacity misses), but leads to a longer hit time at a higher cost and power.
3. **Higher associativity:** will reduce the miss rate (conflict misses) but will increase the hit time.
	1. 2:1 rule of thumb: Direct Mapped with size $N=$ 2-way with size $\frac{N}{2}$
4. [[Multi-Level Cache Architecture]]
5. Prioritize most frequent case: read misses
   - reduce miss penalty
   - write-through cache with write buffer (check write buffer on read, read when write buffer empty)
   - write-back cache (use write buffer when replacing [[Dirty Block|dirty block]])
6. Avoid address translation on cache accesses ([[Virtual Memory]])
   - [[Virtual Cache]]
   - virtually indexed, physically tagged caches