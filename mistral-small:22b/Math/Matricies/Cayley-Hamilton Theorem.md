---
created: '2025-01-31T02:56:50.825207'
modified: '2025-01-31T02:56:50.825210'
source: '[[Cayley-Hamilton Theorem]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Cayley-Hamilton Theorem

## Cayley-Hamilton Theorem

- Every square matrix satisfies it's own characteristic equation
- Characteristic polynomial:
	- $P(\lambda)=(-1)^n\lambda^{n-1}+C_{n-1}\lambda^{n-2}+C_{n-2}\lambda^{n-2}\dots +C_{1}\lambda+C_{0}$
- Characteristic Equation:$P(A)=0$
	- $P(A)=-1^nA^n+C_{n-1}A^{n-1}+\dots C_{1}A+C_{0}$



### Find Inverse of an matrix and $A^8$ for the given matrix A

$$A=
\begin{bmatrix}
1 & 2 \\
2 & -1
\end{bmatrix}
$$

$$
\begin{bmatrix}
1-\lambda & 2 \\
2 & -1-\lambda
\end{bmatrix}=0

$$
$(1-\lambda)(-1-\lambda)-4=0$
$\lambda^2-5=0$
$A^2-5I=0$
$$
A^2=\begin{bmatrix}
5 & 0 \\
0 & 5
\end{bmatrix}
$$
$A^{-1}(A^2-5I)=0$
$A^{-1}A^2-5A^{-1}I=0$
$A=5A^{-1}$
$A^{-1}=\frac{1}{5}A$
$$A^{-1}=\frac{1}{5}\cdot\begin{bmatrix}
1 & 2 \\
2 & -1
\end{bmatrix}$$

$A^8=5^8I$


### Test the C-H theorem of a matrix
$$
A=\begin{bmatrix}
1 & 2 \\
-1 & 3
\end{bmatrix}
$$
and hence  $A^6-4A^5+8A^4-12A^3+14A^2$ is a linear polynomial in A

$A-\lambda I=0$
$\lambda^2-4\lambda+5$
$A^2-4A+5I$
$$

A^2=\begin{bmatrix}
-1 & 8 \\
-4 & 7
\end{bmatrix}
$$
$$
\begin{bmatrix}
-1 & 8 \\
-4 & 7
\end{bmatrix}+4\cdot\begin{bmatrix}
1 & 2 \\
-1 & 3
\end{bmatrix}+5I
$$
Satisfies 0=0


$A^2=4A-5I$

$(4A-5I)^3$

$(4A-5I)^3-4A(4A-5I)^2+8A(4A-5I)-12A(4A-5I)+14(4A-5I)$
$$(4A−5I)^3−4A(4A−5I)^2−4A(4A−5I)+14(4A−5I)$$


