[[Hazard|Hazards]] that originate from memory dependencies, where [[Memory Instructions|Load/Store instructions]] access the same [[Memory|memory locations]]. To generate a hazard, the involved load/store instructions should access the memory [[Out-Of-Order Execution|out-of-order]].

## Types
All of these occur only due to out-of-order execution. Thus, these are not an issue for the integer or [[Floating Point Pipeline|floating point pipelines]], but will become a problem with [[Dynamic Scheduling]] , in particular with [[Tomasulo's Algorithm]] without the [[Reorder Buffer|reorder buffer]]. With the reorder buffer only RAW is allowed.

### Read after Write
Store instruction accessing a location directly before a load instruction reads the same location.

### Write after Write
Two stores instructions writing to a location back-to-back.

### Write after Read
A load instruction reading from a location directly before a store instruction writes to it.