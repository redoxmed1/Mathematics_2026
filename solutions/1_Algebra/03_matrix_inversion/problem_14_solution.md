### Exercise 14. A Matrix That Is Its Own Inverse

**Problem**

Assume that a square matrix A satisfies A² = I. Show that A⁻¹ = A. Then give an example of a 2 × 2 matrix different from I and −I that satisfies this condition, and verify it by multiplication.

**Solution**

The condition A² = I means

$$
AA=I.
$$

By definition, a matrix A⁻¹ is a matrix that multiplies with A to give I. Since A itself satisfies AA = I, A is the inverse of itself:

$$
A^{-1}=A.
$$

**Example**

Choose

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}.
$$

This matrix is different from I and −I. Calculate its square:

$$
A^2=
\begin{pmatrix}
0(0)+1(1) & 0(1)+1(0) \\
1(0)+0(1) & 1(1)+0(0)
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I.
$$

Thus A satisfies the given condition, and its inverse is A itself.

---
