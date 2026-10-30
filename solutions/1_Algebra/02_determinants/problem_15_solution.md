### Exercise 15. Combining Determinant Properties

**Problem**

Let A and B be invertible 2 × 2 matrices with

$$
\det A=-2,
\qquad
\det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties used in order and explain why the factors involving B eventually cancel.

**Solution**

Use the determinant property for a product of square matrices:

$$
\det(XYZ)=\det X\det Y\det Z.
$$

Therefore,

$$
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B).
$$

The determinant of an inverse is the reciprocal of the determinant:

$$
\det(B^{-1})=\frac{1}{\det B}=\frac{1}{3}.
$$

A matrix and its transpose have the same determinant:

$$
\det(A^T)=\det A=-2.
$$

Substitute these values:

$$
\begin{aligned}
\det(B^{-1}A^TB)
&=\frac{1}{3}(-2)(3)
\\
&=-2.
\end{aligned}
$$

The factors involving B cancel because the determinant of B⁻¹ is the reciprocal of the determinant of B:

$$
\det(B^{-1})\det(B)=\frac{1}{3}(3)=1.
$$

The final result is therefore

$$
\det(B^{-1}A^TB)=-2.
$$
