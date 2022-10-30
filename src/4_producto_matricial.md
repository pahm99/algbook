# Producto de matrices

Para poder realizar el producto de matrices se tiene que considerar que el numero de coumnas $A$ debe ser igual el numero de renglones de $B$, dado que se esto no se cumple, significa que no tienen el mismo numero de componentes por lo que son incompatibles
$$
A \space dada \space por \space m \times x \\
B \space dada \space por \space n \times p \\
x = n
$$
De lo contrario es posible realizar la multiplicación

Antes de pasar a la representacion de una combinacion linea, podemos realizar la multiplicación de una matriz multiplicando cada renglon de $A$ por cada una de las columnas de $B$, lo que nos otorga las nuevas componentes, que son coladas por renglones
$$
BA = 
\begin{bmatrix}
3 & -2 \\
5 & 6 
\end{bmatrix}
\begin{bmatrix}
1 & 3 \\
-2 & 4
\end{bmatrix}
=
\begin{bmatrix}
(3 \cdot 1) + (-2 \cdot -2 ) & (3 \cdot 3) + (-2 \cdot 4)\\
(5 \cdot 1) +(6 \cdot -2) & (5 \cdot 3) + (6 \cdot 4)
\end{bmatrix}
=
\begin{bmatrix}
3+4 & 9-8 \\
5-12 & 15+24
\end{bmatrix}
\\ \implies 
\begin{bmatrix}
7 & 1 \\
-7 & 39
\end{bmatrix}
$$


Sea $A = (a_{ij})$ una matriz $m \times n$ y $B = (b_{ij})$ una matriz $n \times p$. Entonces el producto de $A$ y $B$ es una matriz $m \times p$, $C = c_{ij}$  en donde $c_{ij} = (renglon\ i\ de\ A)(columna\ j\ de\ B)$ 

Es decir, el elemento $ij$ de $AB$ es el producto punto del renglón $i$ de $A$ y la de la columna $j$ de $B$. Obteniendo
$$
C_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + \cdots + a_{in}b_{nj}
$$
Asi si el numero de columnas de $A$ es igual al de renglones de $B$, por lo tanto $A$ y $B$ sin compatibles con la multiplicación
$$
C_{ij} = \sum_k^n \ a_{ik}\ b_{kj}
$$
Prodriamos decir que el producto de matrices no conmuta.  $AB \neq BA$.

## Ejemplo de "Contacto directo e indirecto con una enfermedad contagiosa"

El ejemplo dice : Suponga que 4 individuos entran en contacto con 6 individuos de un segundo grupo. Estos contactos, llamados contactos directos, pueden representarse mediante una matriz $4\times6$
$$
A = \begin{bmatrix}
0 & 1 & 0 & 0 & 1 & 0 \\
1 & 0 & 0 & 1 & 0 & 1 \\
0 & 0 & 0 & 1 & 1 & 0 \\
1 & 0 & 0 & 0 & 0 & 1 \\
\end{bmatrix}\ \\
$$
En este caso $a_{ij} = 1$ *si la* $i-esima$ persona del primer grupo entra en contacto con la $j-esima$ del segundo grupo. Por ejemplo, el 1 en la posición (2,4) significa que la segunda persona del primer grupo entro en contacto con la 4 persona del segundo grupo. Supongamos un tercer grupo de cinco personas que tienen varios contactos directos con individuos del segundo grupo. Estos se pueden representar mediante una matriz $6\times5$...
$$
B = \begin{bmatrix}
0 & 0 & 1 & 0 & 1 \\
0 & 0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 & 0 \\
1 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 1 & 0 \\
0 & 0 & 1 & 0 & 0 \\
\end{bmatrix}\ \\
$$
Los contactos indirectos o de segundo orden individuos del primer y tercer grupo se representan mediante una matriz $4\times5$ 
$$
C = AB
$$
para ver esto observe que una persona del grupo 3 puede quedar infectado por una del grupo 2, quien a su ves se infecto por una del grupo 1.
$$
a_{24} = 1 \ \ \ y\ \ \ b_{45} = 1
$$
donde se ve que, indirectamente la persona del grupo 3 tuvo contacto con la segunda persona del 1. El total de contactos indirectos entre la segunda persona del grupo 1 y la quinta persona del grupo 3 esta dados por:
$$
C_{25} = \sum_k^n \ a_{2k}\ b_{k5}\\
= 2
$$
de modo que los contactos indirectos será dado por la matriz
$$
C = AB = \begin{bmatrix}
0 & 0 & 0 & 2 & 0 \\
1 & 0 & 2 & 0 & 2 \\
1 & 0 & 0 & 1 & 1 \\
0 & 0 & 2 & 0 & 1 \\
\end{bmatrix}\ \\
$$
Las matrices en general no conmutan pero se pueden asociar.

## Teorema

Sea $A = (a_{ij})$ una matriz $n\times m$, $B=(b_{ij})$ una matriz $m\times p$ y $C = (c_{ij})$ una matriz $p\times q$. Entonces la ley asociativa nos dice que 
$$
(AB)C = A(BC)
$$
y se cumple que $ABC$, definida por cualquiera de los lados de la ecuación es una matriz $n\times q$.

