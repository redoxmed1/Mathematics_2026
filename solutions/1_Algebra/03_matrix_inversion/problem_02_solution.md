### Exercise 2. Formula for a 2×2 Matrix

**Problem**

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
$$

using the formula for a 2 × 2 matrix. At the end, check the result by computing one product with A.

**Solution**

For a matrix

$$
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix},
$$

the determinant is ad − bc. If the determinant is nonzero, its inverse is

$$
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}.
$$

For the given matrix,

$$
\det A=3(4)-2(5)=12-10=2.
$$

Since the determinant is nonzero, the inverse exists. Substitute a = 3, b = 2, c = 5, and d = 4:

$$
A^{-1}
=\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}.
$$

**Verification**

Multiply A by the proposed inverse:

$$
AA^{-1}
=
\begin{pmatrix}
3(2)+2\left(-\frac{5}{2}\right) &
3(-1)+2\left(\frac{3}{2}\right) \\
5(2)+4\left(-\frac{5}{2}\right) &
5(-1)+4\left(\frac{3}{2}\right)
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

The product is I, so the calculated inverse is correct.

---
