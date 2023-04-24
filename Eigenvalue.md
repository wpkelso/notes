#mathematics #differential_equations 
Represented using the Greek letter $\lambda$, an eigenvalue is the factor by which a corresponding [[Eigenvector|eigenvector]] is scaled. They become particularly important in solving [[Partial Differential Equation|partial differential equations]] using the method of [[Separation of Variables Method|separation of variables]]

>[!note] Eigenvalue and Eigenvector Relationship
>$$Av=\lambda A$$ where A is the Eigenvector and $\lambda$ is the eigenvalue. Essentially, Multiplying by an eigenvalue is the same as multiplying by a constant.

## Solving for Eigenvalues
1. Given an eigenvector $A$ $$\begin{bmatrix}a&b\\c&d\end{bmatrix}$$
2. Take the determinant of the vector $$\begin{bmatrix}a-\lambda &b\\c&d-\lambda\end{bmatrix}$$
4. Solve determinant for 0
5. Solve $A-\lambda_1 I$, $A-\lambda_{2}I$ for the roots (where the equation equals $\begin{bmatrix}0\\0\end{bmatrix}$) $X_{1}\text{ and }X_{2}$