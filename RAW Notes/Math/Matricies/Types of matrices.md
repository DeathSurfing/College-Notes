## Types of matrices
The course covers 11 types of matrices:
- Row matrix
- Column matrix
- Square matrix
- Rectangular matrix
- Null matrix
- Diagonal matrix
- Scalar matrix 
- Identity/Unit matrix
- Upper triangular matrix
- Symmetric matrix


### Row matrix
- A matrix having 1 row and n number of columns is called a row matrix.
$$
\begin{bmatrix}
a & b & c & d
\end{bmatrix}_{1\times4}
$$
### Column matrix
- A matrix having 1 column and n number of rows is called a column matrix
$$
\begin{bmatrix}
a \\
b \\
c \\
d
\end{bmatrix}_{4\times1}
$$

### Square matrix
- A matrix where number of rows and column are equal

$$
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}_{2\times2}
$$

### Rectangular matrix
- A matrix where number of rows and column are not equal
$$
\begin{bmatrix}
a & b & c \\
d & e & f
\end{bmatrix}_{2\times3}
$$
$$Or$$
$$
\begin{bmatrix}
a & b \\
c & d \\
e & f
\end{bmatrix}_{3\times2}
$$

### Null matrix or zero matrix
- A matrix in which all the elements contained have the value '0'
$$
\begin{bmatrix}
0 & 0 \\
0 & 0
\end{bmatrix}_{2\times2}
$$



### Diagonal matrix:
- A square matrix in which the diagonal values are non zero and every other value is zero
$$
D=\begin{bmatrix}
a & 0 & 0 \\
0 & b & 0 \\
0 & 0 & c
\end{bmatrix}_{3\times3}
$$



### Scalar matrix
- A Diagonal matrix in which all the diagonal have the same value
$$
D=\begin{bmatrix}
a & 0 & 0 \\
0 & a & 0 \\
0 & 0 & a
\end{bmatrix}_{3\times3}
$$

### Identity / Unit Matrix
- A scalar matrix in which all the diagonal matrix have the value of '1'; it is denoted with ( I )

$$
I_2=\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}_{2\times2}
$$
$$I_{3}=
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}_{3\times3}
$$

### Upper Triangular matrix
- A square matrix in which the values above the diagonal are occupied
$$
U=\begin{bmatrix}
a_{11} & a_{12} & a_{13} \\
0 & a_{22} & a_{23} \\
0 & 0 & a_{33}
\end{bmatrix}_{3\times3}
$$

### Lower Triangular matrix
- A square matrix in which the values below the diagonal are occupied

$$
L=\begin{bmatrix}
a_{11} & 0 & 0 \\
a_{21} & a_{22} & 0 \\
a_{31} & a_{32} & a_{33}
\end{bmatrix}_{3\times3}
$$
### Symmetric matrix
- A square matrix in which the transpose and the matrix are the same
$$A=
\begin{bmatrix}
1 & 2 & 3 \\
2 & 4 & 5 \\
3 & 5 & 6
\end{bmatrix}_{3\times3}
$$
$$A^T=
\begin{bmatrix}
1 & 2 & 3 \\
2 & 4 & 5 \\
3 & 5 & 6
\end{bmatrix}_{3\times3}
$$
$$A=A^T$$