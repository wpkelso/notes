#computer_architecture 
Sitting between the [[Computer Processor|processor]] and the [[Computer Memory|memory]], the cache is a hardware controlled buffer for fast data access. When a [[Memory Instructions|memory instruction]] makes a call to the cache first, checking to see if the data is stored there. If it is, the cache will “hit” and return the word of data. However, if the cache has a “miss” and the data is not in the cache, the call will move to the memory/disk. This disk will return the appropriate [[Memory Block|block]] which will then be stored in the cache. The cache has a larger size than the [[Register|register block]], but a slower access time than a register.

## Principle of Locality
The idea that programs access a relatively small portion of the address space at any instant of time.
>[!info] Two types of Locality
>- **Temporal Locality**: if an item is referenced, it will tend to be referenced again soon
>- **Spatial Locality**: if an item is referenced, items whose addresses are close by are likely to be referenced soon

## Attributes
- Size = Block Size $*$ Number of blocks
- Line/Block Size
- [[Cache Associativity|Associativity]] » Mapping of data blocks to the cache