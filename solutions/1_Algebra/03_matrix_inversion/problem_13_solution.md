### Exercise 13. Undoing a Composite Transformation

**Problem**

The matrices

\[
S=\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},
\qquad
H=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\]

describe nonuniform scaling and shear. For T = HS, find T⁻¹ in two ways:

1. First compute T, then calculate its inverse.
2. Use the property (HS)⁻¹ = S⁻¹H⁻¹.

Compare the results. Additionally, compute H⁻¹S⁻¹ and verify that using the incorrect order gives a different matrix. Explain the rule: "When undoing a composition of operations, we undo them from the end."

**Solution**

**Method 1. Calculate T first, then invert it**

Since T = HS,

\[
T=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1(2)+1(0) & 1(0)+1(1) \\
0(2)+1(0) & 0(0)+1(1)
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}.
\]

Calculate the determinant:

\[
\det(T)=2(1)-1(0)=2.
\]

Since the determinant is nonzero, the inverse exists.

Using the inverse formula for a 2 × 2 matrix:

\[
T^{-1}
=
\frac12
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
\]

**Method 2. Reverse the order of the inverses**

First, calculate the inverse of S and H:

\[
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix}
\]

\[
H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}.
\]

Use the inverse of a product property:

\[
(HS)^{-1}=S^{-1}H^{-1}.
\]

Calculate:

\[
S^{-1}H^{-1}
=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
\]

Both methods give the same result:

\[
T^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
\]

**Check the incorrect order**

Now calculate H⁻¹S⁻¹ without reversing the order:

\[
H^{-1}S^{-1}
=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
\frac12 & -1 \\
0 & 1
\end{pmatrix}.
\]

This result is different from T⁻¹ because the upper-right entry is -1 instead of -1/2.

Therefore, the order of the inverse matrices is important.

**Geometric Explanation**

The transformation T = HS applies S first and then H.

To undo the complete transformation, we must undo H first and then undo S.

This is why the inverse is:

\[
T^{-1}=S^{-1}H^{-1}.
\]

The order of operations is reversed when calculating the inverse of a product.

**Conclusion**

Both methods produce the same inverse matrix:

\[
T^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
\]

The calculation of H⁻¹S⁻¹ gives a different result, confirming that matrix multiplication is not commutative.

The correct rule is:

\[
(AB)^{-1}=B^{-1}A^{-1}.
\]

Therefore, when undoing a composition of transformations, we must reverse the order of the operations.
