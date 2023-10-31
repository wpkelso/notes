---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#computer_architecture 
Type of [[Hazard|hazard]] present in processor datapaths where [[Data Dependence|data dependencies]] are violated by [[Race Condition|race conditions]].

## Handling
Detection & handling occurs during the [[Datapath Design|instruction decoding]] stage.

## Relationships between [[Data Dependence|Data Dependencies]]  and Hazards
*True dependencies* can cause **Read after Write** hazards. *Output dependencies* can cause **Write after Write** hazards. *Anti-dependencies* can cause **Write after Read** hazards.

### Read after Write
All [[Computer Processor|processor]] designs should consider these, except for unpipelined processors.
### Write after Write
Cannot happen in integer [[Pipelining|pipelines]] or pipelines implementing [[Tomasulo's Algorithm]], but can happen in [[Floating Point Pipeline|floating point pipelines]].
### Write after Read
Cannot happen in any previously covered processor designs. (Some designs not covered in yet in these notes may be vulnerable to them however)