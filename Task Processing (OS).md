---
aliases:
  - task processing (OS)
created: 2023-09-08T14:31
updated: 2023-09-12T09:03
---
#programming #operating_systems #embedded_systems  #ECE460 

## Types of Scheduling
- [[Sequence|Sequential]] : Finish one [[Task (OS)|task]] before starting another task
![[Pasted image 20221108143047.png]]
- Concurrent : Task execution can overlap in time, still only working on a single task at a given time
![[Pasted image 20221108143227.png]]
- Parallel : Work on multiple tasks simultaneously
	- Can be sequential or concurrent in nature
![[Pasted image 20221108143245.png]]

Scheduling is implemented via a [[Scheduler (OS)|scheduler]]