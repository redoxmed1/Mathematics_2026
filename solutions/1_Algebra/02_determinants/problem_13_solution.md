### Exercise 13. Determinant by Elimination

**Problem**

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

**Solution**

Use row replacements to obtain an upper triangular matrix. Each row replacement leaves the determinant unchanged.

Start with

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}.
$$

**Step 1.** Apply

$$
R_2\leftarrow R_2-2R_1.
$$

The determinant is unchanged:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2
\end{pmatrix}.
$$

**Step 2.** Apply

$$
R_3\leftarrow R_3-R_1.
$$

The determinant is unchanged again:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1
\end{pmatrix}.
$$

**Step 3.** Apply

$$
R_3\leftarrow R_3+2R_2.
$$

This row replacement also preserves the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}.
$$

The matrix is now upper triangular. Its determinant is

$$
\det A=1(1)(1)=1.
$$

No row swaps or row scalings were used. Every operation was a row replacement, so the determinant remained unchanged throughout the elimination.

---
