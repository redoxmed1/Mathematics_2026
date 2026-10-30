### Exercise 15. Two Methods for Solving the Same System

**Problem**

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
7 \\
8
\end{pmatrix},
$$

solve Ax = b in two ways:

1. using A⁻¹b,
2. using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

**Solution**

**Method 1. Use the inverse matrix**

First calculate the determinant:

$$
\det A=2(3)-1(1)=6-1=5.
$$

Since the determinant is nonzero, A is invertible. Its inverse is

$$
A^{-1}
=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}.
$$

Now calculate x = A⁻¹b:

$$
x=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
7 \\
8
\end{pmatrix}
=
\frac15
\begin{pmatrix}
3(7)-1(8) \\
-1(7)+2(8)
\end{pmatrix}
=
\frac15
\begin{pmatrix}
13 \\
9
\end{pmatrix}.
$$

Therefore,

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95
\end{pmatrix}.
$$

**Method 2. Use Gaussian elimination**

Write the augmented matrix:

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}
$$

Swap the two rows to obtain a leading 1:

$$
R_1\leftrightarrow R_2.
$$

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
2 & 1 & \mid & 7 \\
\end{pmatrix}
$$

Eliminate the first entry in row 2:

$$
R_2\leftarrow R_2-2R_1.
$$

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & -5 & \mid & -9 \\
\end{pmatrix}
$$

Divide row 2 by −5:

$$
R_2\leftarrow -\frac15 R_2.
$$

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & 1 & \mid & \frac95 \\
\end{pmatrix}
$$

Eliminate the second entry in row 1:

$$
R_1\leftarrow R_1-3R_2.
$$

$$
\begin{pmatrix}
1 & 0 & \mid & \frac{13}{5} \\
0 & 1 & \mid & \frac95 \\
\end{pmatrix}
$$

Therefore,

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95
\end{pmatrix}.
$$

**Comparison and verification**

Both methods give the same solution:

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95
\end{pmatrix}.
$$

Check by substituting into the original system:

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{13}{5} \\
\frac95
\end{pmatrix}
=
\begin{pmatrix}
\frac{26}{5}+\frac95 \\
\frac{13}{5}+\frac{27}{5}
\end{pmatrix}
=
\begin{pmatrix}
7 \\
8
\end{pmatrix}
=b.
$$

Both methods require finding the solution and checking it. For this small 2 × 2 system, the inverse method is short because the inverse formula is straightforward. Gaussian elimination is also direct and uses elementary row operations. For larger systems, Gaussian elimination is usually more efficient than calculating a full inverse.
