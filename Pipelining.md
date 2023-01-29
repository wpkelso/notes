#computer_architecture 
A case of [[Instruction-Level Parallelism|instruction-level parallelism]] where different [[Instruction Set Architecture|instructions]] use the [[Computer Processor|processor]] at the same time.

![[Pasted image 20230126140749.png]]
Fig. *An unpipelined [[Designing Datapaths|datapath]] vs a pipelined datapath*

>[!note] 
>Ideally, pipelining means there is one instruction or result every cycle. This is not achieved in practice due to hazards.

## Pipeline Registers
Special purpose registers that store the result of a pipeline stage at the end of each clock cycle as an input of the next stage. These registers exist because of the idea that instructions must not interfere with one another. Some results will need to be propagated from one stage to another if the source and the destination aren't adjacent stages.