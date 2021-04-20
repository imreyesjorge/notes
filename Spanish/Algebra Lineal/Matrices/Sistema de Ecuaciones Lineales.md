# Sistema de Ecuaciones Lineales
Un sistema de $m$ ecuaciones lineales con $n$ incógnitas es un conjunto de $m$ ecuaciones lineales que se puede escribir en la forma:

$$
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = b1,
$$
$$
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = b2,
$$
$$
\vdots
$$
$$
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = b_m
$$

donde las $a_{ij}'s$ y las $b_i's (1 \le i \le 1 \le j \le n)$ son escalares.

Un vector $(s_1, ...., s_n)$ es una **solución del sistema** si es solución de cada una de las ecuaciones del sistema. El **conjunto solución** de un sistema de ecuaciones es el conjunto de todas las soluciones del sistema.

**Resolver** un sistema de ecuaciones significa encontrar el conjunto solución, es decir, encontrar todas las soluciones del sistema.

## Clasificación según las soluciones
Con relación al sistema de ecuaciones, se dice que el sistema es:
- **Consistente y determinado:** si tiene exactamente una solución.
- **Consistente e indeterminado:** si tiene más de una solución.
- **Inconsistente:** si no tiene solución

## Representación Matricial
Considere el sistema de ecuaciones lineales:

$$
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = b1,
$$
$$
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = b2,
$$
$$
\vdots
$$
$$
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = b_m
$$

y sea $A,b \text{ y } [A|b]$ las matrices

$$
A =
\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{bmatrix},

b = 
\begin{bmatrix}
b_1 \\
b_2 \\
\vdots \\
b_m
\end{bmatrix},

[A|b] =
\begin{bmatrix}
\begin{array}{cccc|c}
a_{11} & a_{12} & \dots & a_{1n} & b_1 \\
a_{21} & a_{22} & \dots & a_{2n} & b_2 \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} & b_{m}
\end{array}
\end{bmatrix}
$$

La matriz $A$ es la **matriz de coeficientes**; $b$ es el **vector (o matriz) de términos independientes**; la matriz $[A|b]$ es la **matriz aumentada** asociada con el sistema. Sea $x=(x_1,...,x_n)$. Una versión matricial del sistema es $Ax = b$:

$$
\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{bmatrix}
\begin{bmatrix}
x_1 \\
x_2 \\
\vdots \\
x_n
\end{bmatrix}
=
\begin{bmatrix}
b_1 \\
b_2 \\
\vdots \\
b_m
\end{bmatrix}
$$

La otra versión matricial es:

$$
x_1 
\begin{bmatrix}
a_{11} \\
a_{21} \\
\vdots \\
a_{m1}
\end{bmatrix}
+ x_2
\begin{bmatrix}
a_{12} \\
a_{22} \\
\vdots \\
a_{m2}
\end{bmatrix}
+ \dots + x_n
\begin{bmatrix}
a_{1n} \\
a_{2n} \\
\vdots \\
a_{mn}
\end{bmatrix}
=
\begin{bmatrix}
b_1 \\ b_2 \\ \vdots \\ b_m
\end{bmatrix}
$$

Es decir, $b = Ax = x_1A_{*1} + x_2A_{*2} + \dots + x_nA_{*n},$ donde $A_{*1},A_{*2},...,A_{*n}$ son las columnas de $A$.

## Espacio Columna 
El **espacio columna** de una matriz $A$ de $m \times n$ es la imagen de la función inducida por $A$ y se denota con el símbolo $R(A)$:

$$
R(A) = \{b \in R^m | b = Ax \text{ para algún } x \in R^n\} = \{Ax | x \in R^n\}
$$

## Sistemas de Ecuaciones Equivalentes
Dos sistemas de ecuaciones lineales son **equivalentes** si tienen exactamente el mismo conjunto solución.

## Sistema de Ecuaciones Lineales Homogéneo
Un sistema de $m$ ecuaciones lineales con $n$ incógnitas

$$
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = 0y,
$$
$$
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = 0,
$$
$$
\vdots
$$
$$
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = 0
$$

en el que el vector de términos independientes es cero, se dice que es **homogéneo**. De otra manera se dice que es **no homogéneo**.

## Espacio Nulo
Sea $A$ una matriz de $m \times n$. El **espacio nulo** de la matriz $A$ es el conjunto

$$
N(A) = \{x | Ax = 0\}
$$

En otras palabras el espacio nulo de $A$ es el conjunto de soluciones del sistema homogéneo $Ax = 0$.

## Algoritmo para el cálculo de un conjunto generador para el espacio nulo de una matriz $A$ de $m \times n$ de rango $r$

1. Llevar a la matriz $A$ a su forma escalonada reducida $E$.
2. Si $r = n$, entonces $N(A) = \{0\}$ y el conjunto generador es $\{0\}$
3. Si $r < n$:
	1. Resolver el sistema de ecuaciones $Ex = 0$ considerando únicamente las ecuaciones que corresponden a los **renglones distintos de cero**.
	2. Escriba cada una de las $r$ variables básicas en términos de las $n-r$ variables libres.
	3. Descomponer la solución general en una combinación lineal de $n-r$ vectores $h_1, ..., h_{n-r}$.
	4. $\{h_1, ..., h_r\}$ es un conjunto generador.