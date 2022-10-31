# Operaciones con Matrices

Dado que las matrices son un entidad matemática, solo se pueden realizar las operaciones de suma / resta y multiplicación entre los componentes de las mismas.

## Suma de Matrices

La suma de las matrices solo se puede realizar entre matrices del mismo tamaño, sean  $A=(a_{i,j})$ y una matriz $B=a_{ij}$  dos matrices $m \times n$, la suma de $A + B$ es la matriz $m \times n$ tal que $A + B$ esta dada por


$$
A+B = (a_{ij}+ b_{ij}) =
\begin{bmatrix}
a_{11} +  b_{11} & \cdots & a_{1n} + b_{1n} \\
a_{21} + b_{21} & \cdots & a_{2n} + b_{2n} \\
\vdots & & \vdots\\ 
a_{m1} + b_{m1} & \cdots & a_{mn} + b_{mn}
\end{bmatrix}
$$

Es decir, se suma cada componente de $A$ con su correspondiente componente en $B$, por lo tanto nos da una matriz del mismo tamaño

## Multiplicación de Matrices

La matrices se pueden multiplicar ya sea por un [escalar](./vectores.md#escalar) o bien por otra matriz, sin la limitante de que tenga quer ser del mismo tamaño

 ### Multiplicación por un Escalar

si $B=(b_{ij})$ es un matriz $m \times n$ y si $\alpha$ es un  [escalar](./vectores.md#escalar), entonces la multiplicacion esta dada por 
$$
\alpha B = (\alpha b_{ij}) = 
\begin{bmatrix}
\alpha b_{11} & \alpha b_{12} & \cdots & \alpha b_{1n} \\
\alpha b_{21} & \alpha b_{22} & \cdots & \alpha b_{2n} \\
\vdots & &  & \vdots\\
\alpha b_{mi} & \alpha b_{m2} & \cdots & \alpha b_{mn}
\end{bmatrix}
$$
Es decir que por cada componente de $B$ es multiplicado por el escalar.

## Teoremas

Dado que las componentes de las matrices son  [escalares](./vectores.md#escalar), y por ende tienen ciertas propiedades que pueden ser extraidas a la matriz, haciendo analogia de logica podemos tener las siguientes teoremas de lo anterior visto.

### Identidad

$$
A + 0 = A \\
1A = A \\
$$

$$
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
$$

$$
\\
A + 0 = \begin{bmatrix}
1 + 0 & 2 + 0 & 3 + 0 \\
4 + 0 & 5 + 0 & 6 + 0
\end{bmatrix} =
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
$$

$$
1A = \begin{bmatrix}
1 \cdot 1 & 1 \cdot 2 & 1 \cdot 3 \\
1 \cdot 4 & 1 \cdot 5 & 1 \cdot 6
\end{bmatrix} = 
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
$$



### Dominante

$$
0A = 0
$$

$$
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
$$

$$
0A = A = \begin{bmatrix}
0 \cdot 1 & 0 \cdot 2 & 0 \cdot 3 \\
0 \cdot 4 & 0 \cdot 5 & 0 \cdot 6
\end{bmatrix} =
\begin{bmatrix}
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix} = 0
$$



### Comutativa

$$
A + B = B + A
$$

$$
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}

B = \begin{bmatrix}
4 & 5 & 6 \\
1 & 2 & 3
\end{bmatrix}
$$

$$
A + B = 
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
+ 
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
$$

$$
A + B = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
+ 
\begin{bmatrix}
4 & 5 & 6 \\
1 & 2 & 3
\end{bmatrix} =
\begin{bmatrix}
1+4 & 2+5 & 2+6 \\
4+1 & 5+2 & 6+3
\end{bmatrix} 
= 
\begin{bmatrix}
5 & 7 & 8 \\
5 & 7 & 9
\end{bmatrix}
$$

$$
B+A =
\begin{bmatrix}
4 & 5 & 6 \\
1 & 2 & 3
\end{bmatrix} 
+
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
=
\begin{bmatrix}
4+1 & 5+2 & 6+2 \\
1+4 & 2+5 & 3+2
\end{bmatrix}
= 
\begin{bmatrix}
5 & 7 & 8 \\
5 & 7 & 9
\end{bmatrix}
$$



### Asociativa

$$
(A+B)+C = A+(B+C)
$$

$$
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
\space
B = \begin{bmatrix}
4 & 5 & 6 \\
1 & 2 & 3
\end{bmatrix}

C = \begin{bmatrix}
2 & 3 & 4 \\
5 & 6 & 1
\end{bmatrix}
$$

$$
(A + B) + C = 
(\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
 
+ \begin{bmatrix}
4 & 5 & 6 \\
1 & 2 & 3
\end{bmatrix})
+
\begin{bmatrix}
2 & 3 & 4 \\
5 & 6 & 1
\end{bmatrix}
$$

$$
\implies 
(
\begin{bmatrix}
5 & 7 & 9 \\
5 & 7 & 9
\end{bmatrix}
) +
\begin{bmatrix}
2 & 3 & 4 \\
5 & 6 & 1
\end{bmatrix} 
=
\begin{bmatrix}
7 & 10 & 13 \\
10 & 13 & 10
\end{bmatrix}
$$



### Distributiva

$$
\alpha (A+B) = \alpha A + \alpha B \\
$$

$$
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}

B = \begin{bmatrix}
4 & 5 & 6 \\
1 & 2 & 3
\end{bmatrix}

\alpha = 2
$$

$$
2(A+B) = 2A +2B =
2 \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
+ 
2 \begin{bmatrix}
4 & 5 & 6 \\
1 & 2 & 3
\end{bmatrix}
=
\begin{bmatrix}
2 \cdot 1 & 2 \cdot 2 & 2 \cdot 3 \\
2 \cdot 4 & 2 \cdot 5 & 2 \cdot 6
\end{bmatrix}
+ 
\begin{bmatrix}
2 \cdot 4 & 2 \cdot 5 & 2 \cdot 6 \\
2 \cdot 1 & 2 \cdot 2 & 2 \cdot 3
\end{bmatrix}\\
$$

$$
\implies 2(A+B) = 2A +2B =
\begin{bmatrix}
2 & 4 & 6 \\
8 & 10 & 12
\end{bmatrix}
+ 
\begin{bmatrix}
8 & 10 & 12 \\
1 & 4 & 6
\end{bmatrix}
= 
\begin{bmatrix}
10 & 14 & 18 \\
9 & 14 & 18
\end{bmatrix}
$$

