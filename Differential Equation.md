---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#mathematics 
## Definition
An equation that involves an unknown, where the unknown consists of a function and its derivative(s)

### Simple Examples
	$\text{A) }\frac{dy(dx)}{dx}=0$
	$\text{B) }\frac{dy(x)}{dx}=1$
	$\text{C) }\frac{dy(x)}{dx}=x^n$
	$\text{D) }\frac{dy}{dx}+y=0$

## Types
- [[Ordinary Differential Equation]]
- Partial Differential Equation

## How to Solve
**For A)**
Recall fundamental theorem of calculus
- Indefinite integration $$\int{\frac{dy}{dx}*dx}=\int{0*dx}+C$$
>[!success] Solution
>$$y(x)=0+C, y(x)=C$$

**For B)**
$$\frac{dy}{dx}=1$$
$$\int{\frac{dy}{dx}dx}=\int{1}dx+C$$
>[!success] Solution
>$$y(x)=x+C$$

**For C)**
$n$ *is a parameter*
$$\int{\frac{dy}{dx}dx}=\int{x^n}dx+C$$
$$y(x)=\frac{x^{n+1}}{n+1}+C$$
However, this solution is not valid if n = -1 (due to dividing by zero). Therefore,
$$\text{If }n=-1\text{, }\frac{dy}{dx}=x^{-1}=\frac{1}{x}$$
$$y(x)=\int{\frac{1}{x}dx}+C=log|x|+C$$


>[!success] Solution
>$$y(x)=
>	\begin{cases}
>	 & \frac{x^{n+1}}{n+1}+C &n\neq-1\\
>	 & log|x|+C &n=-1
>	\end{cases}	
>$$

## Notation
If the independent variable is clear, then we can use $y'$ instead of $\frac{dy}{dx} \text{ or } \frac{dy}{dt}$

The **GENERAL SOLUTION** is the a solution with $n$ arbitrary constants. We usually require additional conditions to make the solution unique.

## Explicit vs Implicit Solutions
**Explicit** solutions are solutions where the independent and dependent variables *can* be separated. *i.e.* $\frac{y^2}{2}=C^2-\frac{x^2}{x}$
**Implicit** solutions are solutions where the independent variables *cannot* be separated. *i.e.* $\frac{y^2}{2}+\frac{x^2}{x}=C^2$

## Checking Solutions
Given a function and an ODE, if we plug the function and it's derivatives into the ODE, if the left hand side is identical to the right hand side, then the function is a solution. *i.e.* plug the equation back into the original equation and the sides should match.