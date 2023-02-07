#signal_analysis #mathematics #differential_equations 
Integral transform that converts a function of a real variable (usually $t$ in the time domain) to a function of a complex variable $s$ (in the [[Complex Domain|complex/frequency domain]]).

>[!note] Formula
>$$\mathcal{L}\{f\}(s)=\int^{\infty}_{0}{f(t)e^{st}dt}$$


>[!info] 
>One useful application of the transform is to change [[Ordinary Differential Equation|ordinary differential equations]] into [[Algebra|algebraic]] equations, as well as changing [[Convolution|convolution]] into multiplication.

*To go from the $s$-domain to the time domain, use the [[Inverse Laplace Transform]]*