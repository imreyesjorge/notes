# Método de eliminación de Gauss y Gauss-Jordan

 ## Método de Gauss
 Los pasos del **método de eliminación de Gauss** para llevar una matriz $A \not= 0$ a una forma escalonada son los siguientes:
 
 1. Sea $l$ la primera columna (de izquierda a derecha) de $A$ que no es cero.
 2. Si el primer elemento de la columna $l$ es cero, intercambie el primer renglón por algún renglón debajo de él para tener un primer elemento en la columna $l$ que no sea cero. Se obtiene así una matriz $A_1$ que es equivalente por renglones con la matriz $A$. Al primer elemento en la columna $l$ de $A_1$ le llamaremos **pivote**.
 3. Se use el pivote para eliminar todas las entradas por debajo de esa posición pivotal. Se obtiene así una matriz $A_2$, que es equivalente con la matriz $A_1$ y tal que todas las entradas debajo de la posición pivotal son cero.
 4. Se repite el proceso con la submatriz de $A_2$ que se obtiene al eliminar el primer renglón y las columnas de la $1$ a la $l$.

## Método Gauss-Jordan
Se dice que una matriz $E \in K^{m \times n}$ está en la **forma escalonada reducida por renglones** si:

1. $E$ está en forma escalonada.
2. La primera entrada distinta de cero en cada renglón es $1$ (es decir, cada pivote es $1$).
3. Cada pivote es la única entrada distinta de cero en su columna.

### Algoritmo de Gauss-Jordan para calcular la inversa
Sea $A$ una matriz de $n \times n$:

1. Construya la matriz aumentada $[A|I]$, donde $I$ es la matriz identidad de orden $n$.
2. Lleve la matriz $[A|I]$ a su forma escalonada reducida $[E_A|P]$, donde $E_A$ es la forma escalonada reducida de $A$.
3. Si $E_A=I$, entonces $A$ es invertible y $A^{-1} = P$. En otro caso, $A$ no es invertible.
 
 