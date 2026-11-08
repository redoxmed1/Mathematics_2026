### Exercise 7. Inverse of a Product

**Problem**

Given the matrices:

A =
$$
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

B =
$$
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

Compute $(AB)^{-1}$ and $B^{-1}A^{-1}$.

Check that the results are the same and explain the meaning of the reversed order.

**Solution**

**Step 1. Calculate AB**

$$
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}
$$

**Step 2. Calculate (AB)⁻¹**

$$
\det(AB) = 2(3) - 3(0) = 6
$$

Since the determinant is not zero, the inverse exists.

$$
(AB)^{-1} =
\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
$$

$$
(AB)^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1/3
\end{pmatrix}
$$

**Step 3. Calculate A⁻¹ and B⁻¹**

$$
A^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

$$
B^{-1} =
\begin{pmatrix}
1/2 & 0 \\
0 & 1/3
\end{pmatrix}
$$

**Step 4. Calculate B⁻¹A⁻¹**

$$
B^{-1}A^{-1} =
\begin{pmatrix}
1/2 & 0 \\
0 & 1/3
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

$$
B^{-1}A^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1/3
\end{pmatrix}
$$

**Step 5. Compare the Results**

$$
(AB)^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1/3
\end{pmatrix}
$$

$$
B^{-1}A^{-1} =
\begin{pmatrix}
1/2 & -1/2 \\
0 & 1/3
\end{pmatrix}
$$

Therefore:

$$
\boxed{(AB)^{-1} = B^{-1}A^{-1}}
$$

**Step 6. Explanation**

The inverse of a product reverses the order of multiplication.

When multiplying AB, matrix B acts first, followed by matrix A.

To undo these operations, we must first undo A using A⁻¹ and then undo B using B⁻¹.

This explains why the order is reversed.

**Conclusion**

The calculations confirm that the inverse of a product is equal to the product of the inverses in reversed order.
