# Matrices

una matriz $A$ de $m×n$ es un _arreglo_ rectangular de $mn$ números dispuestos en $m$ columnas y $n$ columnas

$$m = renglones,\space n = columnas$$


$$
A = \begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots \\
a_{mi} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}
$$
las componente $ij$ se denota como $a_{ij}$ y es numero que aparece en renglón $i$ y al columna $j$ de la matriz $A$. La matriz también puede ser escrita como
$$
A = a_{ij}
$$

## Matriz Cuadrada

Si una matriz $m\times n$ donde $m = n$, se le denomina matriz cuadrada.
$$
Ejemplo \\
a_{44} = \begin{bmatrix}
1 & 2 & 3 & 4 \\
5 & 6 & 7 & 8 \\
9 & 10 & 11 & 12 \\
13 & 14 & 15 & 16 \\
\end{bmatrix}
$$

## Matriz Cero

Si todos las componentes de la matriz son cero, se denomina matriz cero
$$
\begin{bmatrix}
0 & 0 & 0\\
0 & 0 & 0
\end{bmatrix}
$$

## Igualdad de Matrices

Dos Matrices $A = (a_{ij})$ y $B = (b_{ij})$ son iguales si

1. Son del mismo tamaño, es decir que el numero de renglones y columnas de $A$ son igual al mismo numero de renglones y columnas de $B$
2. La componentes son iguales, es decir que para cada componente de $A$ en $a_{ij}$ es es igual en $b_{ij}$

### Iguales

$$
\begin{bmatrix}
5 & 3 & 7 \\
2 & 4 & 8
\end{bmatrix} =
\begin{bmatrix}
5 & 3 & 7 \\
2 & 4 & 8
\end{bmatrix}
$$

### No iguales

$$
\\ \begin{bmatrix}
5 & 3 & 7 \\
2 & 4 & 8
\end{bmatrix} =
\begin{bmatrix}
5 & 3 & 10 \\
2 & 4 & 8
\end{bmatrix}\\
$$

$$
\\ \begin{bmatrix}
5 & 3 & 7 \\
2 & 4 & 8
\end{bmatrix} =
\begin{bmatrix}
5 & 3 & 10 \\
2 & 4 & 8 \\
11 & 16 & 12
\end{bmatrix}\\
$$



