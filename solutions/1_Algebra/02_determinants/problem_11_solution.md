### Exercise 11. Shortening the Calculation with Row Operations

**Problem**

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

**Solution**

Start with

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}.
$$

Subtract the first row from the second row:

$$
R_2\leftarrow R_2-R_1.
$$

This row replacement does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 4 & 6
\end{pmatrix}.
$$

Subtract the first row from the third row:

$$
R_3\leftarrow R_3-R_1.
$$

This operation also does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3
\end{pmatrix}.
$$

Subtract twice the second row from the third row:

$$
R_3\leftarrow R_3-2R_2.
$$

This is another determinant-preserving row replacement:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}.
$$

The resulting matrix is upper triangular. Its determinant is the product of the diagonal entries:

$$
\det A=1(1)(1)=1.
$$

Every operation used was a row replacement, so none changed the determinant.

---
