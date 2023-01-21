#mathematics 
## Definition
A [[Differential Equation]] where the unknowns consists of one or more functions of one variable, involving the derivatives of those functions.
>[!note]
>In general, given an $n$th order, the ODE can be written as $$F(x,y,\frac{dy}{dx},\frac{d^2y}{dx^2},...,\frac{d^ny}{dx^n})=0$$
>We have to have the $\frac{d^ny}{dx^n}$ term.

*Ex.*$$\frac{dy}{dx}=ax+b$$
> $x$ is the independent variable
> $y$ is the dependent variable

>[!success] Solution
>$$\int{\frac{dy}{dx}dx}=\int{(ax+b)dx}+C$$
>$$y(x)=\frac{ax^2}{2}+bx+C$$

## Classification
- **Order:** highest level of differentiation
  *Ex.* $y'''+3y=0$ is a 3rd order
- **Linear:** the dependent variable $y(t)$ and it's derivatives $y'(t), y''(t),...$ are linear with respect to $y$
  *Ex.* $a(t)y(t)+b(t)$ is linear with respect to time, \_$y(t)$+\_ is linear with respect to time
  (*There is a special case, where the highest derivative term is linear, but others terms are not, it can be classified as quasi-linear*)
	- **Constant/variable coefficient:** if the coefficient of $y$ or its derivatives is changing (because of another variable), the DE is a variable coefficient 
	  *Ex.* $5x^2y''+3xy'+x^2y=2x^2+1$ is constant variable
	- **Homogeneous/non-homogenous:** if one side is equal to zero, the ODE is homogeneous
	  *Ex.* $5y''+3y'+y=0$ is homogeneous
- **Non-Linear:**
  *Ex.* $2yy''+3x^2y=\sin(x)$
  
*For linear ODEs, we try to find analytic solutions through Quantitative analysis. For non-linear problems, we try to do qualitative analysis.*
>[!note]
>In general an $n$-th order ODE is linear if it has the form $$a_n(x)\frac{d^ny}{dx^n}+a_{n-1}(x)\frac{d^{n-1}y}{dx^{n-1}}+...+a_1\frac{dy}{dx}+a_0(x)y=f(x)$$ as long as $a_{n}(x)\neq 0$
>

>[!note]
>Move all $y, y',...$ terms to the LHS, if the RHS $=0$, homogenous. If not, it's non-homogeneous

## Solution Techniques for First-Order ODEs (Linear & Non-Linear)
*(Trying to find analytic solutions of ODEs)*

>[!question] 
>$$\frac{dy}{dt}=-ky$$
>*1<sup>st</sup> order, linear, constant coefficient, homogeneous ODE*

1. Find the general solution
2. Solution to [[Initial Value Problem]]

>[!question] 
>$$\frac{dy}{dx}=xy$$
