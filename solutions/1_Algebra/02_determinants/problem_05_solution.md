### Exercise 5. Row Operations

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

find the determinant by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

**Solution**

Use row replacements to create zeros below the first entry. A row replacement of the form “one row plus a multiple of another row” does not change the determinant.

Start with

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}.
$$

**Step 1.** Apply

$$
R_2\leftarrow R_2-2R_1.
$$

This operation does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}.
$$

**Step 2.** Apply

$$
R_3\leftarrow R_3+R_1.
$$

This operation also does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}.
$$

The first column now has zeros below the first entry. Expanding along that column gives

$$
\begin{aligned}
\det A
&=
\begin{vmatrix}
-3 & -6 \\
6 & 5
\end{vmatrix}
\\
&=(-3)(5)-(-6)(6)
\\
&=-15+36
\\
&=21.
\end{aligned}
$$

Both operations were row replacements, so the determinant remained unchanged at every step. Thus the original determinant is 21.

---
