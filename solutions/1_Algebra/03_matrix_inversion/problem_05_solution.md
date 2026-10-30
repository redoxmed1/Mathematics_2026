### Exercise 5. A 3×3 Matrix

**Problem**

Use Gauss–Jordan elimination to find the inverse of

$$
A=
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}.
$$

Check the result by multiplication.

**Solution**

Start with the augmented matrix [A | I]:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
1 & 0 & 1 & \mid & 0 & 0 & 1 \\
\end{pmatrix}
$$

**Step 1.** Eliminate the first entry in row 3:

$$
R_3\leftarrow R_3-R_1.
$$

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & -1 & 1 & \mid & -1 & 0 & 1 \\
\end{pmatrix}
$$

**Step 2.** Eliminate the second entry in row 3:

$$
R_3\leftarrow R_3+R_2.
$$

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 2 & \mid & -1 & 1 & 1 \\
\end{pmatrix}
$$

**Step 3.** Make the third pivot equal to 1:

$$
R_3\leftarrow \frac12 R_3.
$$

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}
$$

**Step 4.** Eliminate the third entry in row 2:

$$
R_2\leftarrow R_2-R_3.
$$

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 0 & \mid & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}
$$

**Step 5.** Eliminate the second entry in row 1:

$$
R_1\leftarrow R_1-R_2.
$$

$$
\begin{pmatrix}
1 & 0 & 0 & \mid & \frac12 & -\frac12 & \frac12 \\
0 & 1 & 0 & \mid & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}
$$

The left block is I, so the right block is A⁻¹:

$$
A^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 & \frac12 \\
\frac12 & \frac12 & -\frac12 \\
-\frac12 & \frac12 & \frac12
\end{pmatrix}.
$$

**Verification by multiplication**

Multiply A by A⁻¹. The entries are calculated row by column:

$$
AA^{-1}=
\begin{pmatrix}
1(\frac12)+1(\frac12)+0(-\frac12) &
1(-\frac12)+1(\frac12)+0(\frac12) &
1(\frac12)+1(-\frac12)+0(\frac12) \\
0(\frac12)+1(\frac12)+1(-\frac12) &
0(-\frac12)+1(\frac12)+1(\frac12) &
0(\frac12)+1(-\frac12)+1(\frac12) \\
1(\frac12)+0(\frac12)+1(-\frac12) &
1(-\frac12)+0(\frac12)+1(\frac12) &
1(\frac12)+0(-\frac12)+1(\frac12)
\end{pmatrix}
$$

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
=I.
$$

The product is the identity matrix, confirming the inverse.

---
