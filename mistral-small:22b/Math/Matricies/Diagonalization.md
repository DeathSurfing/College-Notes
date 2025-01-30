---
created: '2025-01-31T02:56:50.826212'
modified: '2025-01-31T02:56:50.826215'
source: '[[Diagonalization]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Diagonalization

## Diagonalization :

- Take two similar matrices
	- must have the same order matrix
- Then we can generate the diagonalization between the two matrices
TLDR Converting $A\to B$ or $B\to A$


If it satisfies the conditions:
- Both matrices are square matrices
- There exists a non zero matrix
- The linearly independent vectors can be called a modal matrix

Let there be two matrices A and B and "p" (non zero Eigen vector)

$AP = BP$
$P^{-1}AP=B$
$P^{-1}AP=D$

IMPORTANT PROPERTY:
$D^n=P^{-1}A^nP$
$A^n=P^{-1}D^nP$


#### Find a matrix "p" which Diagonalizes it matrix

$$
A=\begin{bmatrix}
4 & 1 \\
2 & 3
\end{bmatrix}
$$ 
Verify that $D=P^{-1}AP$, Where D is a diagonal matrix . Hence find $A^6$


##### Eigen values:
$(4-\lambda)(3-\lambda)-2=0$
$\lambda^2-7\lambda+10=0$
$\lambda={2,5}$

Case 2: $\lambda=2$
$(A-\lambda I)X=0$
$(A-2I)X=0$

$$A=\begin{bmatrix}
4-2 & 1 \\
2 & 3-2
\end{bmatrix}
\times \begin{bmatrix}
x_1 \\
x_2
\end{bmatrix} = 0
$$

$$A=\begin{bmatrix}
2 & 1 \\
2 & 1
\end{bmatrix} \times \begin{bmatrix}
x_1 \\
x_2
\end{bmatrix}=0$$


$$
2v_{1}+v_{2}=0
$$
$$
2v_{1}+v_{2}=0
$$

$$
v_{2}=\begin{bmatrix}
1 \\
-2
\end{bmatrix}
$$

Case 1 : $\lambda=5$
$(A-\lambda I)X=0$
$(A-2I)X=0$

$$A=\begin{bmatrix}
4-5 & 1 \\
2 & 3-5
\end{bmatrix}
\times \begin{bmatrix}
x_1 \\
x_2
\end{bmatrix} = 0
$$
$$
A=\begin{bmatrix}
-1 & 1 \\
2 & -2
\end{bmatrix} \times \begin{bmatrix}
x_1 \\
x_2
\end{bmatrix}=0
$$

$$
v_{1}=\begin{bmatrix}
1 \\
1
\end{bmatrix}
$$

#### Generate Modal matrix P:

$$
P= \begin{bmatrix}
1 & 1 \\
1 & -2
\end{bmatrix}
$$

#### Find $P^{-1}$

$$
P^{-1}=\frac{1}{\det(P)}\times adj(P)
$$

Using Calculator:
$$
P^{-1}=\begin{bmatrix}
\frac{2}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{-1}{3}
\end{bmatrix}
$$
#### Verifying $D=P^{-1}AP$

$$
D=\begin{bmatrix}
5 & 0 \\
0 & 2
\end{bmatrix}
$$


#### Finding $A^6$

$A^6=PD^6P^{-1}$
$$A^6=\begin{bmatrix}
1 & 1 \\
-2 & 1
\end{bmatrix} \times \begin{bmatrix}
5^6 & 0 \\
0 & 2^6
\end{bmatrix} \times \begin{bmatrix}
\frac{2}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{-1}{3}
\end{bmatrix}$$

Using Calculator:

$$
A^6=\begin{bmatrix}
10438 & 5187 \\
-20812 & -10438
\end{bmatrix}


$$