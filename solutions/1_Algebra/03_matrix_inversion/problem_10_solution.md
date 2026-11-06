
# Exercise 10 – Inverse of a Diagonal Matrix

## Problem

Given the following two diagonal matrices:

$$
D =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

$$
E =
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

Without using Gauss-Jordan elimination, determine which matrix is invertible. For the invertible matrix, calculate its inverse and verify the result by multiplication.

---

## Solution

### Step 1: Understand the inverse of a diagonal matrix

A diagonal matrix is invertible if and only if all its diagonal entries are nonzero.

To calculate its inverse, take the reciprocal of each diagonal entry while keeping all other entries equal to zero.

### Step 2: Determine whether D is invertible

The given matrix D is:

$$
D =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

Its diagonal entries are 2, -3, and 5.

Since all three entries are nonzero, matrix D is invertible.

### Step 3: Calculate the inverse of D

Take the reciprocal of each diagonal entry:

$$
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

### Step 4: Verify the inverse by multiplication

To verify the result, multiply D by its inverse:

$$
DD^{-1} =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

Calculate each diagonal entry:

$$
DD^{-1} =
\begin{pmatrix}
2(\frac{1}{2}) & 0 & 0 \\
0 & (-3)(-\frac{1}{3}) & 0 \\
0 & 0 & 5(\frac{1}{5})
\end{pmatrix}
$$

Simplify:

$$
DD^{-1} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
= I
$$

The result is the identity matrix, which confirms that the calculated inverse is correct.

### Step 5: Determine whether E is invertible

The given matrix E is:

$$
E =
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

Its diagonal entries are 2, 0, and 5.

A diagonal matrix cannot be inverted if one of its diagonal entries is zero.

We can also verify this by calculating its determinant:

$$
\det(E) = 2(0)(5) = 0
$$

Since the determinant is zero, matrix E is not invertible.

Therefore, no inverse exists for E.

---

## Conclusion

- Matrix D is invertible because all its diagonal entries are nonzero.
- Its inverse is:

$$
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

- Matrix E is not invertible because one of its diagonal entries is zero.

The multiplication DD inverse gives the identity matrix I, confirming the result.
