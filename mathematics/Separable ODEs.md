---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#mathematics 

> [!info] Definition
> **Separable**
> The right hand side of the [[Ordinary Differential Equation|equation]] can be separated into an $x$ function times a $y$ function

*Ex.*
$$\frac{dy}{dx}=\frac{y-1}{x+3}=(y-1)*\frac{1}{x+3}$$
$$\frac{1}{y-1}dy=\frac{1}{x+3}dx, y\neq1$$
$$\int{\frac{1}{y-1}dy}=\int{\frac{1}{x+3}dx}+C$$
$$\text{Implicit solution: }\log{|y-1|}=\log{|x+3|}+C$$
$$\text{Explicit solution: }$$
---
## Method for Solving
Solving the equation $$\frac{dy}{dx}=g(x)p(y)$$
1. multiply by $dx$ and by $h(y)=\frac{1}{p(y)}$ to obtain $h(y)dy=g(x)dx$
2. integrate both sides $\int h(y)dy=\int g(x)dx$ to get $H(y)=G(x)+C$, an implicit solution to the differential equation