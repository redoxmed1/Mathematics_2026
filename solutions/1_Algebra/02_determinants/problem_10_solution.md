### Exercise 10. Detecting Dependence

**Problem**

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5
\end{pmatrix}
=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

**Solution**

The second row is exactly twice the first row:

$$
(2,4,6)=2(1,2,3).
$$

Therefore, the rows are linearly dependent. A square matrix with linearly dependent rows has determinant zero.

Consequently,

$$
\det A=0.
$$

A square matrix with determinant zero is not invertible. Thus the matrix is singular because one row is a multiple of another row.

---
