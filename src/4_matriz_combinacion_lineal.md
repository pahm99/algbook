# Multiplicación de Matrices como una combinación lineal de las columnas de A

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
De lo anterior podemos decir 
$$
c_1 = \begin{bmatrix}
a_{11} \\ a_{12} \\ \vdots \\ a_{1n}
\end{bmatrix}
$$
