## Notación de la sumatoria.

Sean $a_{n}$ y $b_n$ dos sucesiones reales y $C$ un numero real. Entonces
$$
\sum_{k=M}^N \ Ca_{k} =  C\sum_{k=M}^N \ a_{k}
$$

$$
\sum_{k=M}^N \ (a_k \pm b_k) =  \sum_{k=M}^N \ a_{k} \pm \sum_{k=M}^N \ b_{k}
$$

$$
\sum_{k=M}^N \ (a_k) =  \sum_{k=M}^m \ a_{k} +\sum_{k=m}^M \ a_{k}\\ Si \ M<m<N
$$

# Producto de vectores por Sumatoria

$$
a= \begin{bmatrix} a_1 & a_2 & a_3 \end{bmatrix} \quad
b = \begin{bmatrix} b_1 \\ b_2  \\ b_3 \end{bmatrix} \\
\sum_{k = 1}^n a_kb_k = a_1b_1 + a_2b_2 + a_3a_3 + ... + a_nb_n
$$

# Producto de Matrices por Sumatoria

$$
A = \begin{bmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23}
\end{bmatrix}
\quad
B = \begin{bmatrix}
b_{11} & b_{12} & b_{13} \\
b_{21} & b_{22} & b_{24} \\
b_{31} & b_{32} & b_{34}
\end{bmatrix}
\\ sea \space C = AB
\\
c_{11} = a_{11}b_{11} + a_{12}b_{21} + a_{13}b_{31} = \sum_{k=1}^3 a_{1k}b_{k1} \\
\\
c_{12} = a_{11}b_{12} + a_{12}b_{22} + a_{13}b_{32} = \sum_{k=1}^3 a_{1k}b_{k2}
\\ \implies  \\
cij = \sum_{k = 1}^n a_{ik}b_{kj}
$$

