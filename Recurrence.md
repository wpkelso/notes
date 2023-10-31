---
tags:
  - mathematics
  - discrete_mathematics
created: 2023-09-12T08:45
updated: 2023-09-12T10:31
---

# Recurrence

A [[Formula|formula]] or [[Sequence|sequence]] that is defined using previous elements of the sequence. Perhaps one of the most famous examples of a recurrence is the [[Fibonacci Series]] which is defined using the previous two elements of the sequence.

Given this, the recursive definition of a sequence consists of a recurrence relation and an initial condition.

## Closed Form

The closed form of a recurrence is a [[Function|function]] that is defined to enable solving for some arbitrary element $g_{n}$ without solving for $g_{n-1}, g_{n-2}, \dots, g_{0}$. It entails using a fixed-amount of finite operations on $n$.

## The Characteristic Root Technique

Given a recurrence relation $a_{n}+\alpha a_{n-1}+\beta a_{n-1}=0$, we can define a [[Characteristic Polynomial|characteristic polynomial]] for the relation. Given this characteristic polynomial, we can apply the two distinct roots and assume the closed form solution of the recurrence is $$a_{n}=ar_{1}^{n}+br_{2}^{n}$$ where $a$ and $b$ are constants determined by the initial conditions.

>[!info] 
>This is similar to a method for solving second order homogeneous linear [[Ordinary Differential Equation|ordinary differential equations]], including the solutions for repeated roots. (Complex roots most likely don’t exist for recurrence relations).

