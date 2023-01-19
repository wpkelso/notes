#mathematics 
An [[Ordinary Differential Equation]] together with an initial condition which specifies the value of the unknown function at a given point in the domain.

In any general solution there should be $n$ arbitrary constants. Therefore, we need $n$ conditions to solve the solution, of type $y^x(0)$.

*Ex.* $\frac{dy}{dx}=-k(y-y_r)$, $y(0)=70$
	**General Solution:**$$y(t)=Ce^{-kt}+y_r$$
>	Plug in $t=0$, $y(0)=70$
>	$70=C*1+y_r$, $c=70-y_r$
>	We set the unique solution $y(t)=(70-y_r)e^{-kt}+y_r$
>	
	
## Example of a Special IVP
$$
\begin{cases}
 & \frac{dy}{dx}=f(x,y) \\
 & y(x_0)=y_0 \\
\end{cases}
$$
>[!success] Solution
>$$
>\begin{cases} \\
> & x=x \\
> & y=y(x)
>\end{cases}
$$

*This solution is also called a trajectory*
