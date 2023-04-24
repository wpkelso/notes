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

### n-Bit [[Saturation Arithmetic|Saturating]] Counters
The use of counters relies on the idea that a branch will tend to do the same thing in close succession, and thus predicting the behavior of a branch based on it’s recent behavior is going to be more successful.

![[Pasted image 20230422180134.png]]