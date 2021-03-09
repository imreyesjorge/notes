# Suma y Resta de Matrices
La suma y resta de matrices son operaciones sencillas de realizar, veremos una seguida de la otra.

## Suma
Para realizar la suma de una matriz, bastará con seguir la formula $[C]_{ij} = [A]_{ij} + [B]_{ij}$, lo cual nos quedaría de una forma más general de la siguiente forma:

$$
\begin{bmatrix}
a_{11} & \dots & a_{1n} \\
a_{21} & \dots & a_{2n} \\
\vdots & & \vdots \\
a_{m1} & \dots & a_{mn}
\end{bmatrix}
+
\begin{bmatrix}
b_{11} & \dots & b_{1n} \\
b_{21} & \dots & b_{2n} \\
\vdots & & \vdots \\
b_{m1} & \dots & b_{mn}
\end{bmatrix}
=
\begin{bmatrix}
a_{11} + b_{11} & \dots & a_{1n} + b_{1n} \\
a_{21} + b_{21} & \dots & a_{2n} + b_{2n} \\
\vdots & & \vdots \\
a_{m1} + b_{m1} & \dots & a_{mn} + b_{mn}
\end{bmatrix}
$$

### Propiedades de la suma
- $A + B = B + A$
- $A + (B +C) = (A + B) + C$
- $A + 0 = A$
- $A + (-A) = 0$
- $c(A + B) = cA +cB$
- $(c_1 + c_2)A = c_1A + c_2A$
- $c_1(c_2A) = (c_1c_2)A$ 
- $1 * A = A$
- $(-1)A = -A$
- $0A = 0$
- $c0 = 0$

## Resta

Para realizar la resta de una matriz, bastará con seguir la formula $[C]_{ij} = [A]_{ij} - [B]_{ij}$, lo cual nos quedaría de una forma más general de la siguiente forma:

$$
\begin{bmatrix}
a_{11} & \dots & a_{1n} \\
a_{21} & \dots & a_{2n} \\
\vdots & & \vdots \\
a_{m1} & \dots & a_{mn}
\end{bmatrix}
-
\begin{bmatrix}
b_{11} & \dots & b_{1n} \\
b_{21} & \dots & b_{2n} \\
\vdots & & \vdots \\
b_{m1} & \dots & b_{mn}
\end{bmatrix}
=
\begin{bmatrix}
a_{11} - b_{11} & \dots & a_{1n} - b_{1n} \\
a_{21} - b_{21} & \dots & a_{2n} - b_{2n} \\
\vdots & & \vdots \\
a_{m1} - b_{m1} & \dots & a_{mn} - b_{mn}
\end{bmatrix}
$$