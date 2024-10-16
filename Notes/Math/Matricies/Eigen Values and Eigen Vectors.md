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
**Case 1**: For $\lambda=2$

$[A-2I]X=0$
$$A=\begin{bmatrix}
-4-2 & -6 \\
3 & 5-2
\end{bmatrix}$$
$$\begin{bmatrix}
-6 & -6 \\
3 & 3
\end{bmatrix}\times\begin{bmatrix}
x_{1} \\
x_{2}
\end{bmatrix}=0$$
$-6x_{1}-6x_{2}=0$
$3x_{1}+3x_{2}=0$

$x_{1}=-x_{2}$
$let\ x_{2}=t_{1}$
$x_{1}=-t$
$$V_{1}=\begin{bmatrix}
x_{1} \\
x_{2}
\end{bmatrix}=\begin{bmatrix}
-t \\
t
\end{bmatrix},t\in R^n$$

**Case 2:** For $\lambda=-1$

  

$$A = \begin{bmatrix}

5+1 & -6 \\

3 & 7+1

\end{bmatrix}$$
$$\begin{bmatrix} 

6 & -6 \\ 3 & 8 \\ \end{bmatrix}\times\begin{bmatrix}

x_{1} \\ x_{2} \\ \end{bmatrix}=0$$
$6x_1-6x_2=0$
$3x_1+8x_2=0$
$x_1=\frac{-4}{3}x_2$
Let $x_2=t_2$
$x_1=-\frac{4}{3}t_2$
  

$$V_{2} =\begin{bmatrix}

x_{1} \\

x_{2}

\end{bmatrix}$ = $\begin{bmatrix}-\frac{4}{3}t_2\\ t_2 \end{bmatrix}, t_2 

\in R^n$$

### Algebraic multiplicity of Eigen Values
- Eigen values are distinct $\lambda={1,2,3\dots}$
	- Algebraic multiplicity of 
		- $\lambda = 1; AM=1$
		- $\lambda = 2; AM=1$
		- $\lambda = 3; AM=1$

- Eigen Values are repeated $\lambda=2,2,2$
	- Algebraic multiplicity of 
		- $\lambda=2;AM=3$

### Geometric multiplicity of Eigen values
- $\text{Eigen VectorFind correpsonding eigen value}$
- $\lambda=3, (A-\lambda I)X=0,x\in R^n$
- - $\lambda=3, (A-3I)X=0,x\in R^n$
$$\to\begin{bmatrix}
x_1 \\
x_2
\end{bmatrix}=t_1\cdot\begin{bmatrix}
1 \\
-1
\end{bmatrix}+t_{2}\cdot\begin{bmatrix}
0 \\
1
\end{bmatrix}$$
Therefore, there are two vector spaces
thus the geometric multiplicity is 2





$$
A=\begin{bmatrix}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 0 & 4
\end{bmatrix}
$$

$$
Eigen \ Values=2,3,4
$$

$\lambda=2 ;AM=1$
$\lambda=3 ;AM=1$
$\lambda=4 ;AM=1$


for a diagonal matrix the geometric multiplicity is the same as a algebraic multiplicity


### HW:
#### Question 1:
$$
A=\begin{bmatrix}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & -3 & 3
\end{bmatrix}
$$
Find AM and GM

$$
A=\begin{bmatrix}
1 & -3 & 3 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$
$$
A=\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

$\lambda=1,1,1$

$\lambda=1;AM=3$

$$
(A-\lambda I)X=0

$$
$$
\begin{bmatrix}
-1 & 1 & 0 \\
0 & -1 & 1 \\
1 & -3 & 2
\end{bmatrix} \times\begin{bmatrix}
x_1 \\
x_2 \\
x_3
\end{bmatrix}=\begin{bmatrix}
0 \\
0 \\
0
\end{bmatrix}
$$

$x_{1}=x_{2}$
$x_{2}=x_{3}$
therefore ,
$x_{1}=x_{2}=x_{3}$
let $x_{1}=x_{2}=x_{3}=t$
$$v_{1}=\begin{bmatrix}
x_1 \\
x_2 \\
x_3
\end{bmatrix}=\begin{bmatrix}
t_1 \\
t_2 \\
t_3
\end{bmatrix}$$
$\lambda=1;GM=1$




#### Question 2:

Determine the algebraic multiplicities and geometric multiplicities of the following 3x3 matrix

$$
A=\begin{bmatrix}
1 & 2 & 2 \\
0 & 2 & 1 \\
-1 & 2 & 2
\end{bmatrix}
$$
$$
\begin{bmatrix}
2 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$
$\lambda=2,2,1$

$$\lambda=2:$$
$AM=2$
$GM=1$
$$\lambda=1$$
$AM=1$
$GM=2$


