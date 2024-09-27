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



## Homework
### Question 1:

We are given the matrix:

$$
A=\begin{bmatrix}
0 & 3 & -6 & 6 & 4 & -5 \\
3 & -7 & 8 & -5 & 8 & 9 \\
3 & -9 & 12 & -9 & 6 & 15
\end{bmatrix}
$$

**Step 1**: Swap row 1 and row 2 to get a non-zero leading entry in the first row:

$$
R_1 \leftrightarrow R_2
$$

$$
A_1=\begin{bmatrix}
3 & -7 & 8 & -5 & 8 & 9 \\
0 & 3 & -6 & 6 & 4 & -5 \\
3 & -9 & 12 & -9 & 6 & 15
\end{bmatrix}
$$

**Step 2**: Subtract row 1 from row 3 to create a zero in the first column of row 3:

$$
R_3 \leftarrow R_3 - R_1
$$

$$
A_2=\begin{bmatrix}
3 & -7 & 8 & -5 & 8 & 9 \\
0 & 3 & -6 & 6 & 4 & -5 \\
0 & -2 & 4 & -4 & -2 & 6
\end{bmatrix}
$$

**Step 3**: Multiply row 1 by \(\frac{1}{3}\) to make the leading coefficient of row 1 a 1:

$$
R_1 \leftarrow \frac{1}{3}R_1
$$

$$
A_3=\begin{bmatrix}
1 & -\frac{7}{3} & \frac{8}{3} & -\frac{5}{3} & \frac{8}{3} & 3 \\
0 & 3 & -6 & 6 & 4 & -5 \\
0 & -2 & 4 & -4 & -2 & 6
\end{bmatrix}
$$

**Step 4**: Multiply row 2 by \(\frac{1}{3}\) to make the leading coefficient of row 2 a 1:

$$
R_2 \leftarrow \frac{1}{3}R_2
$$

$$
A_4=\begin{bmatrix}
1 & -\frac{7}{3} & \frac{8}{3} & -\frac{5}{3} & \frac{8}{3} & 3 \\
0 & 1 & -2 & 2 & \frac{4}{3} & -\frac{5}{3} \\
0 & -2 & 4 & -4 & -2 & 6
\end{bmatrix}
$$

**Step 5**: Add 2 times row 2 to row 3 to make the leading coefficient in row 3, column 2, a zero:

$$
R_3 \leftarrow R_3 + 2R_2
$$

$$
A_5=\begin{bmatrix}
1 & -\frac{7}{3} & \frac{8}{3} & -\frac{5}{3} & \frac{8}{3} & 3 \\
0 & 1 & -2 & 2 & \frac{4}{3} & -\frac{5}{3} \\
0 & 0 & 0 & 0 & 0 & 0
\end{bmatrix}
$$

**Step 6**: Add 7/3 times row 2 to row 1 to eliminate the leading coefficient in column 2 of row 1:

$$
R_1 \leftarrow R_1 + \frac{7}{3}R_2
$$

$$
A_6=\begin{bmatrix}
1 & 0 & -\frac{2}{3} & \frac{1}{3} & 2 & 1 \\
0 & 1 & -2 & 2 & \frac{4}{3} & -\frac{5}{3} \\
0 & 0 & 0 & 0 & 0 & 0
\end{bmatrix}
$$


### Question 2:


We are given the matrix:

$$
A=\begin{bmatrix}
1 & -2 & 3 & 9 \\
-1 & 3 & 0 & -4 \\
2 & -5 & 5 & 17
\end{bmatrix}
$$

**Step 1**: Add row 1 to row 2 to create a zero in the first column of row 2:

$$
R_2 \leftarrow R_2 + R_1
$$

$$
A_1=\begin{bmatrix}
1 & -2 & 3 & 9 \\
0 & 1 & 3 & 5 \\
2 & -5 & 5 & 17
\end{bmatrix}
$$

**Step 2**: Subtract 2 times row 1 from row 3 to create a zero in the first column of row 3:

$$
R_3 \leftarrow R_3 - 2R_1
$$

$$
A_2=\begin{bmatrix}
1 & -2 & 3 & 9 \\
0 & 1 & 3 & 5 \\
0 & -1 & -1 & -1
\end{bmatrix}
$$

**Step 3**: Add row 2 to row 3 to create a zero in the second column of row 3:

$$
R_3 \leftarrow R_3 + R_2
$$

$$
A_3=\begin{bmatrix}
1 & -2 & 3 & 9 \\
0 & 1 & 3 & 5 \\
0 & 0 & 2 & 4
\end{bmatrix}
$$

**Step 4**: Multiply row 3 by \(\frac{1}{2}\) to make the leading coefficient in row 3 a 1:

$$
R_3 \leftarrow \frac{1}{2}R_3
$$

$$
A_4=\begin{bmatrix}
1 & -2 & 3 & 9 \\
0 & 1 & 3 & 5 \\
0 & 0 & 1 & 2
\end{bmatrix}
$$

**Step 5**: Subtract 3 times row 3 from row 2 to create a zero in the third column of row 2:

$$
R_2 \leftarrow R_2 - 3R_3
$$

$$
A_5=\begin{bmatrix}
1 & -2 & 3 & 9 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 2
\end{bmatrix}
$$

**Step 6**: Subtract 3 times row 3 from row 1 to create a zero in the third column of row 1:

$$
R_1 \leftarrow R_1 - 3R_3
$$

$$
A_6=\begin{bmatrix}
1 & -2 & 0 & 3 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 2
\end{bmatrix}
$$

**Step 7**: Add 2 times row 2 to row 1 to eliminate the leading coefficient in column 2 of row 1:

$$
R_1 \leftarrow R_1 + 2R_2
$$

$$
A_7=\begin{bmatrix}
1 & 0 & 0 & 1 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 2
\end{bmatrix}
$$

The matrix is now in RREF.


## Determinant of a matrix:

- Can only be found for square matricies

- Take the first element of the top row and multiply it by it's minor of a matrix(all values that aren't in the same row or column)
- Subtract the sub matrix(product of the second element) and it's minors 
- Continue to alternate between first and second step until entire matrix is covered.


$$A=\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}$$
$$ det(A)= |A| = a\cdot d -b \cdot c $$
$$B=\begin{bmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{bmatrix}$$
$$det(B)=a \cdot\begin{bmatrix}
e & f \\
h & i
\end{bmatrix}-b\begin{bmatrix}
d & f \\
g & i
\end{bmatrix}+c\begin{bmatrix}
d & e \\
g & h
\end{bmatrix}$$
$$=a(ei-hf)-b(di-gf)+c(dh-eg)$$

### Properties of Determinants:
- If determinant of a matrix is non zero ; the matrix is invertible
- If determinant of a matrix is zero, the matrix is singular

## Rank of a matrix:
- The maximum number of linearly independent rows or columns.

$$Denoted\ by\ \rho(A)$$

### Methods to find a rank of a matrix
- Using Row Echelon form
- Using  Reduced Row Echelon Form
- Minors of discriminants


#### Using Row Reduction Echelon forms
- Transform the matrix into a Row Echelon form
- Determine the rank using the non zero rows

#### Minors of discriminants
- Find the largest square sub matrix (minor) with a non zero determinant
- Only for square matrices

#### Importance of Rank of matrix (USES)
- The Rank of a unit matrix $m\times n$ is $m\ or \ n$
- If a matrix A is of order $m\times n$ then $\rho(A) = min(m,n)$
- If a matrix A is of order $m\times n$ and $|A| \neq 0$ thus $\rho(A)=m$
- If a matrix A is of order $m\times n$ and $|A|=0$ then $\rho(A)$ will be lesser than m

## Find the Rank of the matrix for the following Matrix
$$
\begin{bmatrix}
1 & 2 & 3 \\
2 & 1 & 4 \\
3 & 0 & 5
\end{bmatrix}

$$
## Linear Equation
- The degree of a linear equation is one
- There is no multiplication between two independent variables

### Consistency of Non Homogeneous system of equation:
- Must have at least one solution
- A system is inconsistent if it has no solutions

## Independent system of equation
- Exactly one solution
- Indicates the intersection of two lines

## Dependent system of equation
- Has more than one solution
- Indicates multiple intersections between two functions

### Two Variables:
- the equations are dependent if one equation is a multiple of another
- Dependent systems have an infinite number of solutions
- Every point is a solution





| Types of system              | Example                                     | Nature of Solution                                        | Graphic                                                                              |
| ---------------------------- | ------------------------------------------- | --------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Dependent, Consistent        | $x+y=2$ $2x+2y=4$<br>$\not\in \forall 0=0$  | Infinite number of solutions. They are the same for all   | Both lines will coincide with each other![[Screenshot 2024-09-25 at 4.59.07 PM.png]] |
| Independent,<br>Consistent   | $x+2y=5$<br>$-2x+y=15$<br>$x=-5\ or \ y=-5$ | **Unique Solution**, The lines are intersect at one point | Intersection at one point<br>![[Screenshot 2024-09-25 at 5.00.02 PM.png]]            |
| Independent and inconsistent | $2x+5y=27$<br>$6x+15y=39$<br>$0=-42$        | No solution the lines are parallel                        | ![[Screenshot 2024-09-25 at 5.03.06 PM.png]]                                         |



### System of linear Equation (Non homogeneous system)

- Consider the system of non homogeneous linear equations "n" unknowns and "m" equations

$a_{11}n_{1}+a_{12}n_{2}+a_{13}n_{3}\dots a_{1n}x_{n}=b_{1}$
$a_{21}n_{1}+a_{22}n_{2}+a_{23}n_{3}\dots a_{2n}x_{n}=b_{2}$
$a_{31}n_{1}+a_{32}n_{2}+a_{33}n_{3}\dots a_{3n}x_{n}=b_{3}$
$a_{m1}n_{1}+a_{m2}n_{2}+a_{m3}n_{3}\dots a_{mn}x_{n}=b_{n}$

$$\begin{bmatrix}
a_{11} & a_{12} & a_{13} & ... & a_{1n} \\
a_{21} & a_{22} & a_{23} & ... & a_{2n} \\
a_{31} & a_{32} & a_{33} & ... & a_{3n} \\ 
a_{m1} & a_{m2} & a_{m3} & ... & a_{mn} \\
\end{bmatrix}\times\begin{bmatrix}
x_1 \\
x_2 \\
x_3 \\
x_{m}
\end{bmatrix}=\begin{bmatrix}
b_1 \\
b_2 \\
b_3 \\
b_{m}
\end{bmatrix}$$




##  To find the rank of a matrix and a augmented matrix

- If $\rho(A)=\rho[A|B]=r=n(Number\ of \ unknowns)$
	- Then System is consistent with unique solution
- If $\rho(A)=\rho[A|B]=r<n(Number\ of \ unknowns)$
	- Then System is consistent with infinite solutions
	- $n-r+1$ Solutions are linearly independent 
- If $\rho(A)\not = \rho(A|B)$
	- Then the System has no solutions

## Eigen Values and Eigen Vectors
- Eigen means proper or latent value or root in german

### Eigen Values:
- A square matrix is set to be the Eigen values of a matrix and X be a vector if it satisfies
- $[A]_{m\times n}\ , \exists x \in R^n,\lambda\to Scaler$
- $AX=\lambda X$
- $AX-\lambda X=0,x \in R^n$
- $[A-\lambda I]X=0\to Charecteristic \ equation$

- $\lambda_{1},\lambda_{2}\lambda_{3}\dots\lambda_{n}\to Eigen \ Values$

### Eigen Vectors:
- Defines the direction of the eigen values 
- $[A-\lambda I]X=0\to Charecteristic \ equation$
- $[A_{n}-\lambda_{n}I_{n}]x_{n}=0$
- $[A-\lambda_{k}I]x_{k}=0$
	- $For\ k =1,2,3,4\dots k$

### Properties of Eigen Values:

#### Determinant of A
$\lambda_{1}\times \lambda_{2}\times \lambda_{3}\dots \lambda_{n}=\det(A)$

#### Trace of matrix A
$\lambda_{1}+\lambda_{2}+\lambda_{3}\dots \lambda_{n}=Trace\ of\ (A)$

#### A To the power of N
$[A]^n_{m\times m}=\lambda^n$


### Example of Eigen Values 

$$A=\begin{bmatrix}
5 & 4 \\
1 & 2
\end{bmatrix}$$
$$X=\begin{bmatrix}
1 \\
-1
\end{bmatrix}$$

$$AX=\begin{bmatrix}
5 & 4 \\
1 & 2
\end{bmatrix}\times\begin{bmatrix}
1 \\
-1
\end{bmatrix}$$
Eigen Values are $$X=\begin{bmatrix}
1 \\
-1
\end{bmatrix}$$







### Find the Eigen values corresponding to the Eigen vector of a matrix A
$$A=\begin{bmatrix}
-4 & -6 \\
3 & 5
\end{bmatrix}$$
$$[A-\lambda I]=0$$
$$\begin{bmatrix}
-4 & -6 \\
3 & 5
\end{bmatrix}-\lambda\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}$$
$$\begin{bmatrix}
-4 & -6 \\
3 & 5
\end{bmatrix}-\begin{bmatrix}
\lambda & 0 \\
0 & \lambda
\end{bmatrix}$$
$$\begin{bmatrix}
-4-\lambda & -6 \\
3 & 5-\lambda
\end{bmatrix}$$
$$\det(A-\lambda I)=|A-\lambda I|$$
$$(5-\lambda)(-4-\lambda)+18$$
$$\lambda^2-\lambda-2$$
$$\lambda=2, \lambda=-1$$





