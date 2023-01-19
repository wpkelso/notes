# Convolution Integral
#signal_analysis 
Related: [[Convolution]]
1. $\sigma (t)$ -> $h(t)$
...
5. $\int x(\tau)\sigma (t-\tau)d\tau$ -> $\int x(\tau)h(t-\tau)d\tau$

**x(t) -> $\int^{\infty}_{-\infty} x(\tau)h(t-\tau)d\tau$ ** or $x(t)$ \* $h(t)$

Essentially just take $x(t)$ or $h(t)$ and shift/scale each term in the equation by each term in the other equation. (*This is valid because of the commutative property of convolution*)

*Convolution of an impulse with ANYTHING is the function shifted/scaled by the same amount as the impulse*

### Alternate Approach
$y(t)=\int ^{\infty}_{\alpha =-\infty} h(\alpha)x(t-\alpha)d\alpha$, where $\alpha$ is the stationary term and $x$ is the transformed term
After applying causality, we get $y(t)=\int ^{t}_{0}x(t-\tau) h(\tau)d\tau$
###### Reflect and Shift
Draw $x(t)$ and $h(t)$ using the same scale on the $\tau$-axis
1. Reflect ($x(\tau)$->$x(-\tau)$)
2. Shift ($x(-\tau)$->$x(t-\tau)$)
	1. Important that the $\tau$ value inside of the parenthases is zero or positive
3. Multiply ($h(\tau)x(t-\tau)$)
4. Integrate ($y(t)=\int ^{t}_{0}x(t-\tau) h(\tau)d\tau$)

Repeat for all values of time $t$ to find $y(t)$
###### Integral Solution
1. Plug $x(t)$ and $h(t)$ into the integral $y(t)=\int ^{t}_{0}x(t) h(t-\tau)d\tau$
2. Solve for each range of t