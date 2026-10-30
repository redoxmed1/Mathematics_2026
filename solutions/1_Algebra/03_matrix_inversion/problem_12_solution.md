### Exercise 12. Finding Inverses Without Starting from Scratch

**Problem**

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}.
$$

Without finding A, compute (3A)⁻¹, (Aᵀ)⁻¹, and (A²)⁻¹. Justify each result using the appropriate property.

**Solution**

Use the standard inverse properties.

**1. Inverse of 3A**

For a nonzero scalar c,

$$
(cA)^{-1}=\frac{1}{c}A^{-1}.
$$

Therefore,

$$
(3A)^{-1}
=\frac13
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac23 & -\frac13 \\
-1 & \frac23
\end{pmatrix}.
$$

**2. Inverse of Aᵀ**

The inverse of a transpose is the transpose of the inverse:

$$
(A^T)^{-1}=(A^{-1})^T.
$$

Thus,

$$
(A^T)^{-1}
=
\begin{pmatrix}
2 & -3 \\
-1 & 2
\end{pmatrix}.
$$

**3. Inverse of A²**

The inverse of a product reverses the order:

$$
(A^2)^{-1}=(AA)^{-1}=A^{-1}A^{-1}.
$$

Calculate the product:

$$
(A^2)^{-1}
=
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
2(2)+(-1)(-3) & 2(-1)+(-1)(2) \\
(-3)(2)+2(-3) & (-3)(-1)+2(2)
\end{pmatrix}
=
\begin{pmatrix}
7 & -4 \\
-12 & 7
\end{pmatrix}.
$$

These results use the scalar, transpose, and product properties of matrix inverses. The original matrix A is not needed.

---
