---
created: '2025-01-31T02:56:50.830547'
modified: '2025-01-31T02:56:50.830550'
source: '[[Determinant of a matrix]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Determinant of a matrix

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