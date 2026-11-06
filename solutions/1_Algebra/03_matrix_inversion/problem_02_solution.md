
# Exercise 2 – Formula for a 2×2 Matrix

## Problem

Find the inverse of the following matrix using the formula for a 2×2 matrix. At the end, verify the result by computing one product with the original matrix.

$$
A =
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
$$

---

## Solution

### Step 1: Write the general formula

For a 2×2 matrix:

$$
A =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

The determinant is calculated using:

$$
\det(A) = ad - bc
$$

If the determinant is nonzero, the inverse matrix is:

$$
A^{-1} =
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

### Step 2: Calculate the determinant

For the given matrix:

$$
a=3,\quad b=2,\quad c=5,\quad d=4
$$

Substitute these values into the determinant formula:

$$
\det(A) = 3(4)-2(5) = 12-10 = 2
$$

Since the determinant is equal to 2 and is not zero, the inverse matrix exists.

### Step 3: Calculate the inverse matrix

Substitute the values into the inverse formula:

$$
A^{-1} =
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
$$

Multiply every element by 1/2:

$$
A^{-1} =
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

---

## Verification

To verify the result, multiply the original matrix by the calculated inverse:

$$
AA^{-1} =
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

Calculate each entry:

$$
AA^{-1} =
\begin{pmatrix}
3(2)+2(-\frac{5}{2}) & 3(-1)+2(\frac{3}{2}) \\
5(2)+4(-\frac{5}{2}) & 5(-1)+4(\frac{3}{2})
\end{pmatrix}
$$

Simplify:

$$
AA^{-1} =
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6
\end{pmatrix}
$$

Therefore:

$$
AA^{-1} =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I
$$

Since the product is the identity matrix I, the calculated inverse is correct.

---

## Final Answer

$$
A^{-1} =
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$
