___

## Who discovered the matrix?
The term matrix was coined in the 19th ce (1850) by the english mathematician James Sylvester with the help of Arthur Caylen

Arthur Caylen is known as father of matrices

## What is a matrix?
A rectangular array containing; numbers, symbols and or characters is called a matrix

## Example of a matrix:
$$
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

Rows are showcased by the letter (m) and columns are showcased by (n);

- Rows are horizontal
- Columns are vertical
$$[P]_{m\cdot n}$$
## Order of matrix:

The order of a matrix is represented as the number of rows(m) & the number of coloumns(n).

$$
\begin{bmatrix}
a & b & c \\
d & e & f
\end{bmatrix}_{2\cdot3} 
$$
$$
\begin{bmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{bmatrix}_{3\cdot2}
$$

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

## Homework: How to use of QR code by the use of matrices:

- 117 x 117 pixels
- Showcased by 0 or 1 in black or white
- 3 11x11 pixels to showcase orientation
- Encoded using Reid solemn
- Has 4 levels of error correction (L,H,M,Q)


## Some other types of matrices:
### Skew Matrix (Anti-Symmetric matrix):
- A square matrix whose transpose is equal to it's negative.
$$A=-A^T$$
- All diagonal elements of a skew symmetric matrix are 0
$$A=\begin{bmatrix}
0 & -2 & -3 \\
2 & 0 & -4 \\
3 & 4 & 0
\end{bmatrix}$$
$$-A^T=\begin{bmatrix}
0 & -2 & -3 \\
2 & 0 & -4 \\
3 & 4 & 0
\end{bmatrix}$$
### Idempotent Matrix:
- Matrix satisfies the equation 
- $$A^2=A$$
- $$A^2-A=0$$
- Example:

	  $$A=\begin{bmatrix}
1 & 0 \\
0 & 0
\end{bmatrix}$$
$$A^2=\begin{bmatrix}
1 & 0 \\
0 & 0
\end{bmatrix}\cdot\begin{bmatrix}
1 & 0 \\
0 & 0
\end{bmatrix}$$
$$A^2=\begin{bmatrix}
1 & 0 \\
0 & 0
\end{bmatrix}$$$$A^2=A$$


### Involuntary matrix:
-  Reflexive matrix
- A square matrix
- Matrix equation Satisfies of the same order :
$$A^2=I$$
- Example:
$$A=\begin{bmatrix}
4 & -1 \\
15 & -4
\end{bmatrix}$$
$$A^2=\begin{bmatrix}
4 & -1 \\
15 & -4
\end{bmatrix}\cdot \begin{bmatrix}
4 & -1 \\
15 & -4
\end{bmatrix}$$
$$A^2=\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}$$
$$A^2=I$$


### Transpose matrix:
- A matrix in which rows are changed into columns and vise versa .
- Denoted as 
- $$A^T\ or\ A^t$$
- $$A=\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
0 & 0 & 8
\end{bmatrix}$$
$$A^T=\begin{bmatrix}
1 & 4 & 0 \\
2 & 5 & 0 \\
3 & 6 & 8
\end{bmatrix}$$
### Orthogonal matrix:
- A square matrix
- Satisfies the equation
- $$AA^T=A^TA=I$$
- Example:$$A=\begin{bmatrix}
0 & -1 \\
1 & 0
\end{bmatrix}$$
$$A^T=\begin{bmatrix}
0 & 1 \\
-1 & 0
\end{bmatrix}$$
$$A\cdot A^T=\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}$$
## Elementary Operations:
The elementary operations or transformations of a matrix are the operations performed on rows and columns of a matrix to transform the given matrix into a different form in order to make the calculation easier.

We know that elementary row operations are the operations performed on the rows of matrix. Similarly, elementary column operations are the operations performed on the columns of matrix

### Types of elementary Operations:
- Interchange of rows or columns
- Multiplication of rows or columns by any non zero number
- Add the results to the any row or column

### Echelon form
Refers to a specific arrangement of a matrix; used to simplify solving system of linear equations, and performing matrix operations ; there are two commonly used echelon forms:
- Row Echelon form (REF)
- Reduced Row Echelon form (RREF)

### Row Echelon Form
- Satisfies the conditions : 
	- Leading entries
		- The leading (first non zero ) term of each row is to the right of the leading entry of the row above it
	- Leading entry is one 
		- The leading entry of each (called a pivot) is any number of row echelon form
	- 0 below pivots
		- All values below a pivot are to be made into a zero.
	- All zero rows at bottom
		- all zero rows must be present at the bottom most row
$$A=\begin{bmatrix}
1 & 2 & 3 & 4 \\
0 & 1 & -2 & -8 \\
0 & 0 & 1 & 5
\end{bmatrix}$$



### Reduced Row Echelon Form
- Must satisfy all row echelon form conditions
- Leading entry is one (1)
- Zero's are above and below pivots
	- Pivot's must be the only non zero entry in it's column

$$A=\begin{bmatrix}
1 & 0 & 0 & 4 \\
0 & 1 & 0 & -8 \\
0 & 0 & 1 & 5
\end{bmatrix}$$




