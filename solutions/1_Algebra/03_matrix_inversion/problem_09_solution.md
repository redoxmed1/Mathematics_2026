
# Exercise 9 – Matrix Equation

## Problem

Given the following matrices:

$$
A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Solve the matrix equation AX = B for X.

Before calculating, decide on which side of the equation the inverse of A must be used. Then verify the result by calculating AX.

---

## Solution

### Step 1: Decide where to multiply by the inverse

The unknown matrix X is multiplied by A on its left.

Therefore, we must multiply both sides of the equation on the left by A inverse:

$$
A^{-1}AX = A^{-1}B
$$

Since the product of A inverse and A is the identity matrix I:

$$
A^{-1}A = I
$$

The equation becomes:

$$
IX = A^{-1}B
$$

Therefore:

$$
X = A^{-1}B
$$

### Step 2: Calculate the inverse of A

The given matrix is:

$$
A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

Its determinant is:

$$
\det(A) = 1(1)-2(0) = 1
$$

Since the determinant is not zero, the inverse exists.

Using the 2×2 inverse formula:

$$
A^{-1} =
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
$$

### Step 3: Calculate X

We know that:

$$
X = A^{-1}B
$$

Substitute the matrices:

$$
X =
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Multiply the rows by the columns:

$$
X =
\begin{pmatrix}
1(3)+(-2)(2) & 1(1)+(-2)(4) \\
0(3)+1(2) & 0(1)+1(4)
\end{pmatrix}
$$

Simplify:

$$
X =
\begin{pmatrix}
3-4 & 1-8 \\
0+2 & 0+4
\end{pmatrix}
$$

Therefore:

$$
X =
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

---

## Verification

To verify the result, substitute X into the original equation AX = B:

$$
AX =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

Calculate each entry:

$$
AX =
\begin{pmatrix}
1(-1)+2(2) & 1(-7)+2(4) \\
0(-1)+1(2) & 0(-7)+1(4)
\end{pmatrix}
$$

Simplify:

$$
AX =
\begin{pmatrix}
-1+4 & -7+8 \\
0+2 & 0+4
\end{pmatrix}
$$

Therefore:

$$
AX =
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
= B
$$

The result is equal to the original matrix B, which confirms that the solution is correct.

---

## Conclusion

The solution of the matrix equation AX = B is:

$$
X =
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

The inverse of A must be multiplied on the left because A is positioned on the left side of X in the original equation.

The verification confirms that AX = B.
