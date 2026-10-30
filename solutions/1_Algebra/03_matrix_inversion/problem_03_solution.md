### Exercise 3. When Does the Inverse Not Exist?

**Problem**

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix},
$$

explain in two ways why A⁻¹ does not exist: using the determinant and using dependence between the rows.

**Solution**

**1. Using the determinant**

For a 2 × 2 matrix, the determinant is the product of the main diagonal entries minus the product of the other diagonal entries:

$$
\det A=2(2)-4(1)=4-4=0.
$$

A square matrix is invertible if and only if its determinant is nonzero. Since the determinant is zero, A has no inverse.

**2. Using dependence between the rows**

The first row is (2, 4), and the second row is (1, 2). The first row is twice the second row:

$$
(2,4)=2(1,2).
$$

Thus, the rows are linearly dependent. A matrix with linearly dependent rows is singular and cannot have an inverse.

Both methods give the same conclusion: A⁻¹ does not exist.

---
