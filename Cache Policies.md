#computer_hardware #computer_architecture 
[[Cache]] policies are a set of rules and [[Algorithm|algorithms]] that dictate how a cache handles certain operations such as writes as well as replacement of blocks when needed.

## Replacement Policies
*Replacement policy does not significantly affect miss rate*
- Random
- Least Recently Used (LRU): corollary of temporal locality
	- As LRU is costly, an approximated ‘Psuedo-LRU’ is implemented where 1 bit is allocated for each block in a set and ‘turned on’ or set to 1 when the block is accessed. If all bits are set to 1, then all bits except the most recently accessed are reset. Evictions are done at random to only blocks that have the bit turned off.
- First IN, First OUT (FIFO): may violate temporal locality

## Write Policies
### On Write-Hit
- **Write Through:** write both in cache and in [[Computer Memory|memory]]. This gives a consistent view of memory, is easy to implement, and does not require special handling for evictions; it does however create more memory traffic
- **Write Back:** write only in the cache (requiring a dirty bit). This allows writing at the speed of the cache, with multiple writes terminating in cache and memory being updated only on eviction of a dirty block.

### On Write-Miss
- **Write Allocate:** Allocate the block on write misses, then write the block. This is *usually* used with write-back.
- **No-Write Allocate:** Modify the block only in lower-level memory, so write misses don’t affect the cache. This is *usually* used with write-through.