### Exercise 10. Inverse of a 2x2 Matrix

**Problem**

Given

$$
A=\begin{pmatrix}
3 & 1 \\
5 & 2
\end{pmatrix},
$$

find the inverse matrix $A^{-1}$ using the standard 2x2 inverse formula, and verify that $AA^{-1} = I$.

**Solution**

**1. Compute the determinant**

The determinant of $A$ is:

$$
\det(A) = 3(2) - 1(5) = 6 - 5 = 1.
$$

**2. Apply the inverse formula**

For a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$, the inverse is given by:

$$
A^{-1} = \frac{1}{\det(A)} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix}.
$$

Substituting our values:

$$
A^{-1} = \frac{1}{1} \begin{pmatrix}
2 & -1 \\
-5 & 3
\end{pmatrix}
=
\begin{pmatrix}
2 & -1 \\
-5 & 3
\end{pmatrix}.
$$

**3. Verify the result**

Multiply $A$ by $A^{-1}$ to confirm the product is the identity matrix $I$:

$$
AA^{-1} = 
\begin{pmatrix}
3 & 1 \\
5 & 2
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-5 & 3
\end{pmatrix}
=
\begin{pmatrix}
3(2) + 1(-5) & 3(-1) + 1(3) \\
5(2) + 2(-5) & 5(-1) + 2(3)
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

The result is verified.
