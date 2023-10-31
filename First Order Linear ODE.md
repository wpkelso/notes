---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#mathematics

Classified as a 1st order, linear, variable coefficient [[Ordinary Differential Equation]]

>[!info] General form
>$$a_1(x)\frac{dy}{dx}+a_0(x)y=b(x)$$

## To Solve:
Assume $a_1(x)\neq0$, otherwise there is no ODE.
1. write the equation in the standard form $$\frac{dy}{dx}+P(x)y=Q(x)$$
2. calculate the integrating factor by the formula $$\mu(x)=\exp [\int{P(x)dx}]$$
3. multiply the equation in standard form by $\mu(x)$ and (given the LHS is $\frac{d}{dx}[\mu(x)y]$) get $$\frac{d}{dx}[\mu(x)y]=\mu(x)Q(x)$$
4. integrate the last equation and solve for $y$ to obtain $$y(x)=\frac{1}{\mu(x)}[\int{\mu(x)Q(x)dx}+C]$$