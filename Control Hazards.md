---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#computer_architecture 

Related to [[Control Flow Instructions|control flow instructions]] and in particular branches as the outcome of a branch instruction is not known for a few clock cycles. Thus if a branch is fetched/issued at clock cycle $k$, we cannot issue/fetch a new instruction in clock cycle $k+1$ unless we are using [[Branch Prediction|branch prediction]]. 