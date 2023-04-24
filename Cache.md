#computer_architecture 
Sitting between the [[Computer Processor|processor]] and the [[Computer Memory|memory]], the cache is a hardware controlled buffer for fast data access. When a [[Memory Instructions|memory instruction]] makes a call to the cache first, checking to see if the data is stored there. If it is, the cache will “hit” and return the word of data. However, if the cache has a “miss” and the data is not in the cache, the call will move to the memory/disk, stalling the CPU. This disk will return the appropriate [[Memory Block|block]] which will then be stored in the cache. The cache has a larger size than the [[Register|register block]], but a slower access time than a register.

## Principle of Locality
The idea that programs access a relatively small portion of the address space at any instant of time.
>[!info] Two types of Locality
>- **Temporal Locality**: if an item is referenced, it will tend to be referenced again soon
>- **Spatial Locality**: if an item is referenced, items whose addresses are close by are likely to be referenced soon

## Attributes
- Size = Block Size $*$ Number of blocks
- Line/Block Size
- [[Cache Associativity|Associativity]] » Mapping of data blocks to the cache
- The behavior of the cache can on specific operations can be characterized through it’s [[Cache Policies|various policies]]

## Entries
Each cache entry has the following sections:
1. A block/line of data
2. A tag, allowing us to recognize if the desired block is present
3. Status bits: *valid, dirty,* status for multiprocessors, etc.

## Memory Address Decomposition
- Block offset (depends on block size)
- Index (depends on number of sets)
- Tag (the remainder of the address)
*The Index and the tag together constitute the **block address***

## Checking whether a cache call is a hit or a miss:
1. Check valid bit of validity
2. Follow the index to determine the set
3. Use the tag to check for a match
	- n-way set associative → parallel matches
>[!note] 
>For an $n$-way cache, the number of sets $s$ can be found through the following:
>$$s=\frac{b}{n}=\frac{C}{B*n}$$
>where $b$ is the number of blocks, $C$ is the cache-size, and $B$ is the block-size

## Reads and Writes
For reads, the tag and data block can be read in parallel, and the read can access more bytes than needed. For writes, the block can be modified only after the tag is checked, and only a specific portion of the block is changed.

## Characterizing Cache Performance