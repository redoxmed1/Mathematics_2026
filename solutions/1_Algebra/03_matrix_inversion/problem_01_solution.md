### Exercise 1. Definition of the Inverse

**Problem**

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix},
$$

check, without using a formula, whether B = A⁻¹. Compute AB and BA and relate the result to the definition of the inverse.

**Solution**

A matrix B is the inverse of A if multiplying in either order gives the identity matrix I.

First calculate AB:

$$
AB=
\begin{pmatrix}
2(1)+1(-1) & 2(-1)+1(2) \\
1(1)+1(-1) & 1(-1)+1(2)
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I.
$$

Now calculate BA:

$$
BA=
\begin{pmatrix}
1(2)+(-1)(1) & 1(1)+(-1)(1) \\
(-1)(2)+2(1) & (-1)(1)+2(1)
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I.
$$

Both products equal the identity matrix. Therefore, B is the inverse of A:

$$
B=A^{-1}.
$$

This verifies the definition directly, without using the 2 × 2 inverse formula.

---
