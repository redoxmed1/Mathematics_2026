
# Exercise 7 – Inverse of a Product

## Problem

Given the following matrices:

$$
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

Calculate the inverse of AB and calculate the product of B inverse and A inverse. Check that both results are equal and explain why the inverse of a product reverses the order of the factors.

---

## Solution

### Step 1: Calculate AB

First, multiply matrix A by matrix B:

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

Calculate each entry:

$$
AB =
\begin{pmatrix}
1(2)+1(0) & 1(0)+1(3) \\
0(2)+1(0) & 0(0)+1(3)
\end{pmatrix}
$$

Simplify:

$$
AB =
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}
$$

### Step 2: Calculate the inverse of AB

First, calculate the determinant:

$$
\det(AB) = 2(3)-3(0) = 6
$$

Since the determinant is not zero, the inverse exists.

For a 2×2 matrix, the inverse formula is:

$$
M^{-1} =
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Apply the formula to matrix AB:

$$
(AB)^{-1} =
\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
$$

Simplify:

$$
(AB)^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

### Step 3: Calculate A inverse and B inverse separately

First, calculate the determinant of A:

$$
\det(A) = 1(1)-1(0) = 1
$$

Therefore, the inverse of A is:

$$
A^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Now, calculate the determinant of B:

$$
\det(B) = 2(3)-0(0) = 6
$$

Therefore, the inverse of B is:

$$
B^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
$$

### Step 4: Calculate B inverse multiplied by A inverse

The inverse of a product reverses the order of the matrices.

Calculate:

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Multiply the rows by the columns:

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2}(1)+0(0) & \frac{1}{2}(-1)+0(1) \\
0(1)+\frac{1}{3}(0) & 0(-1)+\frac{1}{3}(1)
\end{pmatrix}
$$

Simplify:

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

### Step 5: Compare both results

From Step 2:

$$
(AB)^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

From Step 4:

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

Both results are equal. Therefore:

$$
(AB)^{-1} = B^{-1}A^{-1}
$$

---

## Explanation

When multiplying ABx, matrix B acts on vector x first, and then matrix A acts on the result.

To reverse these operations, we must undo them in the opposite order.

First, we apply A inverse, and then B inverse.

This can be shown mathematically:

$$
A^{-1}(ABx) = Bx
$$

Then:

$$
B^{-1}A^{-1}(ABx) = x
$$

Therefore, the inverse of a product reverses the order of the original matrices.

---

## Conclusion

The calculations confirm that both methods give the same result:

$$
(AB)^{-1} = B^{-1}A^{-1}
$$

The inverse of a product reverses the order of the factors because the last operation performed must be the first operation undone.
