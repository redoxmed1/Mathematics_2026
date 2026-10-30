### Exercise 6. Solving a System Using the Inverse

**Problem**

Solve Ax = b, where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
5 \\
7
\end{pmatrix},
$$

using x = A⁻¹b. Then substitute the resulting vector back into the equation and check the result.

**Solution**

First calculate the determinant:

$$
\det A=2(3)-1(1)=6-1=5.
$$

Since the determinant is nonzero, A is invertible. Its inverse is

$$
A^{-1}
=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}.
$$

Use x = A⁻¹b:

$$
x=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
5 \\
7
\end{pmatrix}
=
\frac15
\begin{pmatrix}
3(5)-1(7) \\
-1(5)+2(7)
\end{pmatrix}
=
\frac15
\begin{pmatrix}
8 \\
9
\end{pmatrix}.
$$

Therefore,

$$
x=
\begin{pmatrix}
\frac85 \\
\frac95
\end{pmatrix}.
$$

**Verification by substitution**

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac85 \\
\frac95
\end{pmatrix}
=
\begin{pmatrix}
\frac{16}{5}+\frac95 \\
\frac85+\frac{27}{5}
\end{pmatrix}
=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
=b.
$$

The substitution gives the original vector b, so the solution is correct.

---
