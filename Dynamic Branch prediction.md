#computer_hardware 
## Parameters to predict:
- Is this instruction a branch?
- Will it be taken?

## Kinds of Branch Predictors
Use a Branch Prediction Table, which contains history information used for predictions.

Use a Branch Target Buffer, which is a “table” addressed by lower bits of the PC
- lower bits = index; remaining = tag
- BTB stores tags
- Store predictions at icache lines