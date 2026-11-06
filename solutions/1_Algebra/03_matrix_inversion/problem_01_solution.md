
# Exercise 1 – Definition of the Inverse

## Problem

Given the following two matrices:

$$
A =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

Check, without using an inverse formula, whether B is the inverse of A. Calculate both products AB and BA and relate the results to the definition of the inverse matrix.

---

## Solution

A matrix B is the inverse of matrix A if multiplying them in either order gives the identity matrix I.

The definition is:

$$
AB = BA = I
$$

### Step 1: Calculate AB

Multiply matrix A by matrix B:

$$
AB =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

Calculate each entry:

$$
AB =
\begin{pmatrix}
2(1)+1(-1) & 2(-1)+1(2) \\
1(1)+1(-1) & 1(-1)+1(2)
\end{pmatrix}
$$

Simplify:

$$
AB =
\begin{pmatrix}
2-1 & -2+2 \\
1-1 & -1+2
\end{pmatrix}
$$

Therefore:

$$
AB =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I
$$

### Step 2: Calculate BA

Now multiply matrix B by matrix A:

$$
BA =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

Calculate each entry:

$$
BA =
\begin{pmatrix}
1(2)+(-1)(1) & 1(1)+(-1)(1) \\
(-1)(2)+2(1) & (-1)(1)+2(1)
\end{pmatrix}
$$

Simplify:

$$
BA =
\begin{pmatrix}
2-1 & 1-1 \\
-2+2 & -1+2
\end{pmatrix}
$$

Therefore:

$$
BA =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I
$$

---

## Conclusion

Both products give the identity matrix:

$$
AB = BA = I
$$

According to the definition of the inverse matrix, B is the inverse of A.

Therefore:

$$
B = A^{-1}
$$

This confirms that B is the inverse of A without using the 2×2 inverse formula.
