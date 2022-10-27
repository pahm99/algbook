# Combinación lineal.

Sea A una matriz  de $m \times n $ y $x$ un vector de $n \times 1$ , considere la siguiente multiplicación
$$
Ax = 
\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & 	& \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{bmatrix}
\begin{bmatrix}
x_1 \\
x_2 \\
\vdots \\
x_m
\end{bmatrix}
= 
\begin{bmatrix}
a_{11}x_1 & a_{12}x_2 & \cdots & a_{1n}x_n \\
a_{21}x_1 & a_{22}x_2 & \cdots & a_{2n}x_n \\
\vdots & \vdots & 	& \vdots \\
a_{m1}x_1 & a_{m2}x_2 & \dots & a_{mn}x_n
\end{bmatrix}
$$
Lo anterior también se puede mostrar de la siguiente forma, que cada una de las componentes del vector, por cada una de las columnas de la matriz.
$$
x_1
\begin{bmatrix}
a_{11} \\ a_{12} \\ \vdots \\ a_{1n}
\end{bmatrix}
+
x_2
\begin{bmatrix}
a_{12} \\ a_{22} \\ \vdots \\ a_{m2}
\end{bmatrix}
+ \cdots
x_n
\begin{bmatrix}
a_{1n} \\ a_{1n} \\ \vdots \\ a_{mn}
\end{bmatrix}
$$
De lo anterior podemos decir , que $c1$ es igual a la columna 1 de A y $c2$ a la columna 2 y así sucesivamente.
$$
c_1 = \begin{bmatrix}
a_{11} \\ a_{12} \\ \vdots \\ a_{1n}
\end{bmatrix}
&
c2 =
\begin{bmatrix}
a_{12} \\ a_{22} \\ \vdots \\ a_{m2}
\end{bmatrix}
$$
De modo que el producto de de la matriz de A de $m \times x$ y el vector de columnas $x$ es una combinación lineal de las columnas de A
$$
Ax = x_1c_1 + x_xc_2 + \cdots + x_nc_n
$$
Por lo anterior visto, la multiplicación de dos matrices matrices A y B, puede escribirse como la combinación lineal.
$$
Sean A = \begin{bmatrix}
1 & -2 \\
2 & 4 \\
3 & 5 
\end{bmatrix}
&
y
&
B = \begin{bmatrix}
1 & -1 \\
2 & 7
\end{bmatrix}
\implies AB = \begin{bmatrix}
-3 & -15 \\
10 & 26 \\
13 & 32
\end{bmatrix}
$$
Ahora vemos la combinación lineal de las columnas de y b
$$
\begin{bmatrix}
-3 \\
10 \\
13
\end{bmatrix} 
= 1 
\begin{bmatrix}
1 \\
2 \\ 
3
\end{bmatrix} 
+ 2 
\begin{bmatrix}
-2 \\
4 \\ 
5
\end{bmatrix}
$$

$$
\begin{bmatrix}
-3 \\
10 \\
13
\end{bmatrix} 
=
\begin{bmatrix}
1 \cdot 1 \\
1 \cdot 2 \\
1 \cdot 3 
\end{bmatrix}
+
\begin{bmatrix}
2 \cdot -2 \\
2 \cdot 4 \\
2 \cdot 5 
\end{bmatrix}
$$

$$
\begin{bmatrix}
-3 \\
10 \\
13
\end{bmatrix} 
=
\begin{bmatrix}
1 \\
2 \\
3
\end{bmatrix}
+
\begin{bmatrix}
-4 \\
8 \\
10
\end{bmatrix}
$$

$$
\implies 
\begin{bmatrix}
-3 \\
10 \\
13
\end{bmatrix} 
=
\begin{bmatrix}
-3 \\
10 \\
13
\end{bmatrix}
$$

Por lo tanto, podemos conseguir el producto de dos matrices mediante la suma de la combinación lineal de de las columnas de $A$ por cada una de las componentes de cada columna de $B$ ,
$$
C_1 = b_{11}a_1 + b_{21}a_1 + b_{m1}a_1 \\
C_2 = b_{21}a_2 + b_{22}a_2 + b_{m2}a_2 \\
\vdots \\
C_n = b_{mn}a_n + \cdots	
$$
