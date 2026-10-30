### Exercise 11. Parameter and Invertibility

**Problem**

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix},
$$

find all t for which the matrix is invertible, and then give a formula for A(t)⁻¹. Explain what happens to this formula at the excluded values.

**Solution**

Calculate the determinant:

$$
\det A(t)=1(1)-t(t)=1-t^2.
$$

The matrix is invertible when its determinant is nonzero:

$$
1-t^2\neq 0.
$$

Factor the expression:

$$
(1-t)(1+t)\neq 0.
$$

Thus, the matrix is invertible for

$$
t\neq 1
\qquad\mathrm{and}\qquad
t\neq -1.
$$

Using the 2 × 2 inverse formula gives

$$
A(t)^{-1}
=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix},
\qquad t\neq \pm1.
$$

At t = 1 or t = −1, the denominator is zero. The inverse formula is undefined because the original matrix has determinant zero and is not invertible.

---
