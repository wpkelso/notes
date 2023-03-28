#computer_architecture 
Essentially asks, “In how many different positions in the [[Cache|cache]] can a memory block be located?”

## One-Way Caches/Direct Mapped Caches
Each [[Memory|memory]] block can be mapped to one & only one cache block
>[!note] 
>Cache Block = Memory Block Number$\mod{\text{Number of blocks in the cache}}$ 

## Fully Associative Caches
A memory block can be found in any position of the cache

## n-Way Set Associative Caches
A memory block can be found in n positions of the cache
>[!example] 2-way Cache
>Blocks are grouped in “sets”, with the number of blocks in a set == associativity