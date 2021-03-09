# Matriz Nilpotente e Idempotente

## Nilpotente
Una matriz $A \in K^{n \times n}$ es  **nilpotente** si $A^{k} = 0$ para algún entero positivo $k$.

$$
A = 
\begin{bmatrix}
0 & -1 & 2 \\
0 & 0 & 1 \\
0 & 0 & 0
\end{bmatrix}
$$

$$
A^2 =
\begin{bmatrix}
0 & 0 & -1 \\
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}
, \space \space
A^3 = 
\begin{bmatrix}
0 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}
$$

## Idempotente
Una matriz $A \in K^{n \times n}$ es **idempotente** si $A^2 = A$.

$$
\begin{bmatrix}
1 & 1 \\
0 & 0 
\end{bmatrix}
\begin{bmatrix}
1 & 1 \\
0 & 0
\end{bmatrix}
=
\begin{bmatrix}
1 & 1 \\
0 & 0
\end{bmatrix}
$$