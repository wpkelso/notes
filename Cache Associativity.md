---
created: 2023-09-08T14:31
updated: 2023-10-18T08:42
---
#computer_architecture 
Essentially asks, “In how many different positions in the [[Cache|cache]] can a memory block be located?”

## One-Way Caches/Direct Mapped Caches
Each [[Memory|memory]] block can be mapped to one & only one cache block. This maximizes conflicts in the cache.
>[!note] 
>Cache Block = Memory Block Number$\mod{\text{Number of blocks in the cache}}$ 

## Fully Associative Caches
A memory block can be found in any position of the cache. This minimizes the number of conflicts in the cache at the cost of making access more expensive due to the need to check every location in the cache before going to memory. This makes it unsuited for any implementation of decent size, but it is used for some specific scenarios.

## n-Way Set Associative Caches
A memory block can be found in $n$ positions of the cache. 
>[!note]
>Blocks are grouped in “sets”, with the number of blocks in a set == associativity. This means that a memory block can always be found in the $\text{set number} =\text{memory block} \mod{\text{number of sets}}$