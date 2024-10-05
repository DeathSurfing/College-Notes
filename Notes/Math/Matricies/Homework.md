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