# Transpuesta de una matriz
Si $A \in K^{m \times n}$, la **transpuesta** de $A$ es la matriz $A^T$ de $n \times m$ dada por:

$$
[A^T]_{ij} = [A]_{ji}
$$

De manera más visual:

$$
\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \vdots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{bmatrix}^T
=
\begin{bmatrix}
a_{11} & a_{21} & \dots & a_{m1} \\
a_{12} & a_{22} & \dots & a_{m2} \\
\vdots & \vdots & \vdots & \vdots \\
a_{1n} & a_{2n} & \dots & a_{mn}
\end{bmatrix}
$$

## Propiedades
- $(A^T)^T = A$
- $(A + B)^T = A^T + B^T$
- $(cA)^T = cA^T$
- $(AB)^T = B^TA^T$