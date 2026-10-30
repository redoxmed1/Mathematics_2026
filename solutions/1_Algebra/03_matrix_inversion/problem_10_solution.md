### Exercise 10. Inverse of a Diagonal Matrix

**Problem**

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix},
\qquad
E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix},
$$

without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

**Solution**

A diagonal matrix is invertible exactly when every diagonal entry is nonzero. Its inverse is obtained by taking the reciprocal of each diagonal entry.

For D, all diagonal entries 2, −3, and 5 are nonzero. Therefore, D is invertible and

$$
D^{-1}=
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15
\end{pmatrix}.
$$

Check by multiplication:

$$
DD^{-1}=
\begin{pmatrix}
2(\frac12) & 0 & 0 \\
0 & (-3)(-\frac13) & 0 \\
0 & 0 & 5(\frac15)
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
=I.
$$

For E, the middle diagonal entry is zero. Its determinant is the product of its diagonal entries:

$$
\det E=2(0)(5)=0.
$$

Therefore, E is not invertible. No inverse exists for E.

---
