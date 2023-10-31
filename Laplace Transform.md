---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#signal_analysis #mathematics #differential_equations 
Integral transform that converts a function of a real variable (usually $t$ in the time domain) to a function of a complex variable $s$ (in the [[Complex Domain|complex/frequency domain]]).

>[!note] Formula
>$$\mathcal{L}\{f\}(s)=\int^{\infty}_{0}{f(t)e^{st}dt}$$


>[!info] 
>One useful application of the transform is to change [[Differential Equation|differential equations]] into [[Algebra|algebraic]] equations, as well as changing [[Convolution|convolution]] into multiplication.

*To go from the $s$-domain to the time domain, use the [[Inverse Laplace Transform]]*

## Laplace Transform Method for Solving for IVPs
[[Initial Value Problem|IVP]] → [[Laplace Transform]] → [[Algebra|Algebraic Equation]] → [[Inverse Laplace Transform]]

**CHEAT SHEET**
![[Pasted image 20230321163522.png]]