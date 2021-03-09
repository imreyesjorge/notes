# Matrices Triangulares
Se dice que una matriz es **triangular superior** si $[U]_{ij} = 0$ cuando $i>j$. La forma general para las matrices triangulares superiores es:

$$
U =
\begin{bmatrix}
u_{11} & u_{12} & \dots & \dots & u_{1n} \\
0 & u_{22} & \dots & \dots & u_{2n} \\
0 & 0 & \ddots & & \vdots \\
\vdots & \vdots & \ddots & \ddots & u_{n-1,n} \\
0 & 0 & \dots & 0 & u_{nn}
\end{bmatrix}
$$

Se dice que una matriz es **triangular inferior** si $[U]_{ij} = 0$ cuando $i<j$. La forma general para las matrices triangulares superiores es:

$$
U =
\begin{bmatrix}
l_{11} & 0 & 0 & \dots & 0 \\
l_{21} & l_{22} & 0 & \dots & 0 \\
l_{31} & l_{32} & \ddots & \ddots & \vdots \\
\vdots & \vdots & & \ddots & 0 \\
l_{n1} & l_{2n} & \dots & l_{n,n-1} & l_{nn}
\end{bmatrix}
$$