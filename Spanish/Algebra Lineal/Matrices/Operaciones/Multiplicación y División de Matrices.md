# Multiplicación y División de Matrices
La multiplicación y división de matrices es una operación un tanto más compleja a comparación de una simple suma/resta.

## Multiplicación (Producto)
Para que una matriz $A$ de $m \times n$ se pueda multiplicar por una matriz $B$ de $n \times r$ se tiene que cumplir una condición: Las matrices tienen que coincidiar que la parte izquierda de la multiplicación tenga el mismo número de columnas (vertical) que el número de filas (horizontal) de la parte derecha.

> El producto de las matrices no es conmutativo, por lo que si la matriz $A$ ($m \times n$) multiplica a la matriz $B$ ($n \times r$), el producto será posible. Pero en el caso querer multiplicar $B$ por $A$ no necesariamente se podrá ni será el mismo resultado.

El producto de una matriz $A$ por una matriz $B$ denotado $AB$ ó $A*B$ es la matriz de tamaño $m \times r$ cuyas entradas están dadas por:

$$
[AB]_{ij} = \Sigma^{n}_{k=1}[A]_{ik}*[B]_{kj}
$$

### Propiedades del producto
- Propiedad asociativa: $A(BC) = (AB)C$
- Propiedad distributiva: $A(B+C) = AB + AC, (A+B)C = AC + BC$
- Si $A \in K^{m \times n}, I_{m \times m}$ e $I_{n \times n}$ son las matrices identidad de $m \times m$ y $n \times n$, respectivamente:
$$
A_{m \times n}*I_{n \times n} = A_{m \times n}, I_{m \times m}*A_{m \times n} = A_{m \times n}
$$
- $c(AB) = (cA)B = A(cB)$
- $A0 = 0, 0A= 0$
- Si $A \in K^{n \times n}$ y $r, s \in \Bbb{Z} \ge 0$ se tiene: $A^r*A^s =A^{r+s}, (A^r)^s = A^{rs}$ 

## División