---
aliases: ["Orbits Equation"]
---
#mathematics 
**Definition:** If a first order [[Ordinary Differential Equation|ODE]] is a [[Total Differentiation|total differentiation]] of $u(x,y)$, then it is an exact equation and $u(x,y)=C$ is a solution.
>[!info] Formula
>$$N(x,y)\frac{dy}{dx}+M(x,y)=0$$
>Where $N,M$ are two functions of $x,y$

## Method of Discovery
To find whether an equation is an exact equation, 
1. Write the equation in the form as above
2. Multiply by $dx$
3. Take a [[Partial Derivative|partial derivative]] with respect to $x$ of N
4. Take a partial derivative with respect to $y$ of M
5. If the two sides don't match, the equation isn't an exact equation

**Related:** [[Ordinary Differential Equation]]
**Further reading:**
[https://tutorial.math.lamar.edu/classes/de/exact.aspx]

>[!question] *Ex.*
>$$(x^2+3y^2)\frac{dy}{dx}+2xy=0$$
1. Checking the equation is an exact equation
2. Finding $u(x,y)=C$
   $$\frac{\partial u}{\partial x} = M, \frac{\partial u}{\partial y}=N$$
   $$u(x,y)=\int{M(x,y)dx}+C(y)$$
   $$\frac{\partial u}{\partial y}=\frac{\partial}{\partial y}\int{M(x,y)dx}+C'(y)=N$$
$$C(y)=\int{(n-\frac{\partial}{\partial y}\int{Mdx})dx}$$
>[!success] Solution
>$$u(x,y)=yx^2+y^3+C$$

