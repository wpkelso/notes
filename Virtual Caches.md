---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#computer_architecture 

In a virtual [[Cache|cache]], blocks are stored based on virtual addresses. This has the advantage of no memory translation requirement prior to cache access. However, this approach has problems, namely:
- Page-level protection (*solution:* copy protection info in cache)
- Flush on context switch as there are the same virtual addresses for different physical addresses (*solution:* add process-identifier tag)
- [[Aliasing]], where the [[Operating System|OS]] and applications use differnt virtual addresses for the same physical address.
	- Antialiasing hardware guarantees unique physical addresses in cache
	- Page [[Graph Coloring Hueristic|coloring]] in software allowing aliasses to share some address bits
- I/O uses physical addresses

## Virtually-index, Physically Tagged Caches
These avoid some of the issues presented by virtual caches by using part of the untranslated page offset to index cache. This is done in two steps:
1. Access cache using index and translate virtual part of the address in parallel
2. Match tag using physical address
This has the advantage in that the cache read begins immediately and the cache content is based on physical address, but is limited in how large the caches can be.