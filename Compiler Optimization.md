#compilers #programming 
>[!summary] General Idea
>The process of transforming code from one form to another in the hopes it runs faster and with the constraint that it retains the same meaning.

## What constitutes the same meaning?
The same outputs for the same inputs, as well as the failures remaining the same. Optimization should not introduce new exceptions, or hide existing ones. Anything can be optimized, **as long as these rules hold true.**

>[!note] 
>The language may allow some exceptions to be removed, but they should only be removed **if the language specifically allows it.**

## How can we make a program run faster?
- Reduce the number of instructions
- Select or schedule instructions so that they execute in fewer cycles on average
- Co-Design the hardware and the compiler

A compiler is made of many optimizations working together, with each optimization focusing on a single goal. Ordering is important, but there is no magic ordering and we don’t know what’s optimal, so experimentation is required to achieve good orderings.

## Typical Flow in an Optimizer
- Optimizations which enable others come first
- Optimizations which help reduce code size (to reduce runtime of later ones)
- Longer running more complex ones come after simpler ones (loop optimizations)
- Repeat important optimizations multiple times
