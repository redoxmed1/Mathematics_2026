### Exercise 13. Undoing a Composite Transformation

**Problem**

The matrices

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

$$
H =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

describe nonuniform scaling and shear.

For $T = HS$, find $T^{-1}$ in two ways:

1. First compute $T$, then its inverse.
2. Use $(HS)^{-1} = S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix.

Explain the rule: "when undoing a composition of operations, we undo them from the end."

**Solution**

**Step 1. Calculate T = HS**

$$
T = HS =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

$$
T =
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}
$$

**Step 2. Calculate T⁻¹ directly**

First, calculate the determinant:

$$
\det(T) = 2(1) - 1(0) = 2
$$

Since the determinant is not zero, the inverse exists.

Using the formula for the inverse of a 2×2 matrix:

$$
T^{-1} =
\frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
$$

$$
T^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1
\end{pmatrix}
$$

**Step 3. Calculate S⁻¹ and H⁻¹**

The inverse of S is:

$$
S^{-1} =
\begin{pmatrix}
1/2 & 0 \\
0 & 1
\end{pmatrix}
$$

The inverse of H is:

$$
H^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

**Step 4. Calculate S⁻¹H⁻¹ using the inverse of a product**

According to the inverse of a product property:

$$
(HS)^{-1} = S^{-1}H^{-1}
$$

Now multiply:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
1/2 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

$$
S^{-1}H^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1
\end{pmatrix}
$$

**Step 5. Compare the Results**

From the direct calculation:

$$
T^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1
\end{pmatrix}
$$

From the inverse of a product property:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{T^{-1} = S^{-1}H^{-1}}
$$

Both methods give the same result.

**Step 6. Calculate H⁻¹S⁻¹ (Incorrect Order)**

Now calculate the inverse matrices in the opposite order:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1/2 & 0 \\
0 & 1
\end{pmatrix}
$$

$$
H^{-1}S^{-1} =
\begin{pmatrix}
1/2 & -1 \\
0 & 1
\end{pmatrix}
$$

Comparing the results:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1
\end{pmatrix}
$$

$$
H^{-1}S^{-1} =
\begin{pmatrix}
1/2 & -1 \\
0 & 1
\end{pmatrix}
$$

The two matrices are different.

Therefore:

$$
\boxed{S^{-1}H^{-1} \neq H^{-1}S^{-1}}
$$

This confirms that the order of matrix multiplication matters.

**Step 7. Explanation**

The transformation $T = HS$ means that the scaling transformation $S$ is applied first, followed by the shear transformation $H$.

To undo these operations, we must reverse their order.

First, we undo the shear using $H^{-1}$, and then we undo the scaling using $S^{-1}$.

This is why the inverse is:

$$
(HS)^{-1} = S^{-1}H^{-1}
$$

If we use $H^{-1}S^{-1}$ instead, we obtain a different matrix because matrix multiplication is not commutative.

**Conclusion**

The calculations confirm that the inverse of a product is obtained by reversing the order of the inverses.

Both methods give the same result:

$$
\boxed{
T^{-1} = S^{-1}H^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1
\end{pmatrix}
}
$$

The incorrect order, $H^{-1}S^{-1}$, gives a different result.

Therefore, when undoing a composition of operations, we must always undo them from the end.
