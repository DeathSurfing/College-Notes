---
created: '2025-01-31T02:56:50.818400'
modified: '2025-01-31T02:56:50.818403'
source: '[[Some other types of matrices]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Some other types of matrices

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