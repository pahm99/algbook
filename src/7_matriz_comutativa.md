## Ejemplo de dos matrices que so conmutativas

Suponga que las matrices $A$ y $B$ son cuadradas y se hacen particiones conformantes de
$$
C = \begin{bmatrix}
I & A \\
O & I \\
\end{bmatrix} \ D=\begin{bmatrix}
I & B \\
O & I \\
\end{bmatrix}
$$
Muestre que $C$ y $D$ son conmutativas

Aquí $O$ denota a la matriz $O$ y a $I$ como la matriz identidad tal que $AI - A = IA$

### Solución 

$$
CD = \begin{bmatrix}
I & A \\
O & I \\
\end{bmatrix} \ \begin{bmatrix}
I & B \\
O & I \\
\end{bmatrix}\\ CD= \begin{bmatrix}
I^2+AO & IB+AI \\
OI + IO & OB + I^2 \\
\end{bmatrix}\\CD= \begin{bmatrix}
I & B+A \\
O & I \\
\end{bmatrix}
$$

$$
DC = \begin{bmatrix}
I & B \\
O & I \\
\end{bmatrix} \begin{bmatrix}
I & A \\
O & I \\
\end{bmatrix} \ \\ DC= \begin{bmatrix}
I^2+BO & IA+BI \\
OI + IO & OA + I^2 \\
\end{bmatrix}\\DC= \begin{bmatrix}
I & A+B \\
O & I \\
\end{bmatrix}
$$

como $B+A = A + B$ entonces $CD = DC$