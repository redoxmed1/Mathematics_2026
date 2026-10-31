
### Exercise 15. Two Methods for Solving the Same System

**Problem**

Given

$$
A=
\begin{pmatrix}
2 & 1\\
1 & 3
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
7\\
8
\end{pmatrix},
$$

solve $Ax=b$ in two ways:

1. Using $x=A^{-1}b$.
2. Using Gaussian elimination.

Compare both solutions, count the essential arithmetic operations, and identify which method is simpler in this example.

**Solution**

**Method 1. Using the inverse matrix**

First calculate the determinant:

$$
\det(A)=2(3)-1(1)
$$

$$
\det(A)=6-1=5
$$

Since the determinant is nonzero, $A$ is invertible.

Calculate the inverse:

$$
A^{-1}
=
\frac15
\begin{pmatrix}
3 & -1\\
-1 & 2
\end{pmatrix}
$$

$$
A^{-1}
=
\begin{pmatrix}
\frac35 & -\frac15\\
-\frac15 & \frac25
\end{pmatrix}
$$

Now calculate $x=A^{-1}b$:

$$
x=
\begin{pmatrix}
\frac35 & -\frac15\\
-\frac15 & \frac25
\end{pmatrix}
\begin{pmatrix}
7\\
8
\end{pmatrix}
$$

$$
x=
\begin{pmatrix}
\frac35(7)-\frac15(8)\\
-\frac15(7)+\frac25(8)
\end{pmatrix}
$$

$$
x=
\begin{pmatrix}
\frac{21-8}{5}\\
\frac{-7+16}{5}
\end{pmatrix}
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac95
\end{pmatrix}
}
$$

**Arithmetic operation count for Method 1**

1. Determinant: 2 multiplications and 1 subtraction = 3 operations.
2. Calculate the inverse entries: 4 divisions by 5 = 4 operations.
3. Matrix-vector multiplication: 4 multiplications and 2 additions = 6 operations.

Total:

$$
3+4+6=13
$$

Therefore, the inverse method requires 13 arithmetic operations using this counting convention.

**Method 2. Using Gaussian elimination**

Start with the augmented matrix:

$$
\left(
\begin{array}{cc|c}
2 & 1 & 7\\
1 & 3 & 8
\end{array}
\right)
$$

**Step 1. Swap the rows**

$$
R_1\leftrightarrow R_2
$$

The matrix becomes:

$$
\left(
\begin{array}{cc|c}
1 & 3 & 8\\
2 & 1 & 7
\end{array}
\right)
$$

**Step 2. Eliminate the first entry in row 2**

Apply the row operation:

$$
R_2\rightarrow R_2-2R_1
$$

Calculate the new second row:

$$
(2-2(1),\ 1-2(3)\ |\ 7-2(8))
$$

$$
=(0,-5\mid -9)
$$

The matrix becomes:

$$
\left(
\begin{array}{cc|c}
1 & 3 & 8\\
0 & -5 & -9
\end{array}
\right)
$$

**Step 3. Make the second pivot equal to 1**

Apply:

$$
R_2\rightarrow -\frac15R_2
$$

The matrix becomes:

$$
\left(
\begin{array}{cc|c}
1 & 3 & 8\\
0 & 1 & \frac95
\end{array}
\right)
$$

**Step 4. Eliminate the second entry in row 1**

Apply:

$$
R_1\rightarrow R_1-3R_2
$$

The matrix becomes:

$$
\left(
\begin{array}{cc|c}
1 & 0 & \frac{13}{5}\\
0 & 1 & \frac95
\end{array}
\right)
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac95
\end{pmatrix}
}
$$

**Arithmetic operation count for Method 2**

1. Row interchange: no scalar arithmetic operations.
2. First elimination: 3 multiplications and 3 subtractions = 6 operations.
3. Normalize the second row: 3 scalar multiplications = 3 operations.
4. Second elimination: 3 multiplications and 3 subtractions = 6 operations.

Total:

$$
6+3+6=15
$$

Therefore, Gaussian elimination requires 15 arithmetic operations using the same counting convention.

**Comparison of both methods**

| Method | Arithmetic operations |
|---|---:|
| Inverse matrix method | 13 |
| Gaussian elimination | 15 |

Both methods produce the same solution:

$$
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac95
\end{pmatrix}
$$

The inverse method requires 13 arithmetic operations, while Gaussian elimination requires 15.

The difference is:

$$
15-13=2
$$

Therefore, the inverse method requires 2 fewer arithmetic operations in this particular example.

However, Gaussian elimination is generally more practical for larger systems because it avoids calculating the complete inverse matrix.

**Final verification**

Substitute the solution into the original equation:

$$
Ax=
\begin{pmatrix}
2 & 1\\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{13}{5}\\
\frac95
\end{pmatrix}
$$

$$
Ax=
\begin{pmatrix}
\frac{26}{5}+\frac95\\
\frac{13}{5}+\frac{27}{5}
\end{pmatrix}
$$

$$
Ax=
\begin{pmatrix}
\frac{35}{5}\\
\frac{40}{5}
\end{pmatrix}
=
\begin{pmatrix}
7\\
8
\end{pmatrix}
=b
$$

The verification confirms that the solution is correct.

**Conclusion**

Both methods solve the system correctly. The inverse method is slightly simpler for this particular example according to the arithmetic operation count. Gaussian elimination is generally preferable for larger systems.

