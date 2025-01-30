---
created: '2025-01-31T02:56:50.829618'
modified: '2025-01-31T02:56:50.829620'
source: '[[Elementary Operations]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Elementary Operations

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