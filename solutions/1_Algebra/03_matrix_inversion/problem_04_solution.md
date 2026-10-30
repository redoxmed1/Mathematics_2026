### Exercise 4. Gauss–Jordan

**Problem**

Find A⁻¹ using the Gauss–Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}.
$$

Show the augmented matrix [A | I] after successive operations and explain why obtaining I on the left gives the inverse on the right.

**Solution**

Start by placing the identity matrix to the right of A:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

**Step 1.** Make the lower-left entry zero using

$$
R_2\leftarrow R_2-3R_1.
$$

The augmented matrix becomes

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

**Step 2.** Make the second pivot equal to 1:

$$
R_2\leftarrow -R_2.
$$

This gives

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

**Step 3.** Make the upper-right entry in the left block zero:

$$
R_1\leftarrow R_1-2R_2.
$$

The result is

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

The left block is now I. The same row operations have transformed the original A into I, so they have transformed the right-hand identity block into the matrix that multiplies A to give I. Therefore,

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}.
$$

---
