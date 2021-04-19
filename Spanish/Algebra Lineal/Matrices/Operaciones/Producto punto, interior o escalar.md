# Producto punto, interior o escalar
Sean $x = (x_1, ..., x_n)$ y $y = (y_1, ..., y_n)$ vectores columna del mismo tamaño. Entonces el **producto punto**, **producto interno** o **producto escalar** de $x$ e $y$, denotado por $x \cdot y$ o por $\langle x,y\rangle$ es el escalar $x^Ty$:

$$
x \cdot y := 
\begin{bmatrix}
x_1 & x_2 & \dots & x_n
\end{bmatrix}
\begin{bmatrix}
y_1 \\
y_2 \\
\vdots \\
y_n
\end{bmatrix}
= x_1y_1 + x_2y_2 + \dots + x_ny_n
$$

## Propiedades del producto punto o interior
El producto punto satisface las siguientes propiedades:

1. $x \cdot y = y \cdot x$
2. $x \cdot (y + z) = x \cdot y + x \cdot z$
3. $x \cdot (cy) = c(x \cdot y), c$ un número.
4. $x \cdot x > 0$ si $x \not= 0$