### Exercise 9. Matrix Equation

**Problem**

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix},
$$

solve the equation AX = B for X. Before calculating, decide on which side of the equation A⁻¹ must be used. Then check the result by computing AX.

**Solution**

The unknown matrix X is multiplied by A on its left. Therefore, multiply both sides on the left by A⁻¹:

$$
A^{-1}AX=A^{-1}B.
$$

Since A⁻¹A = I, this gives

$$
X=A^{-1}B.
$$

The inverse of A is

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}.
$$

Now multiply:

$$
X=
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
=
\begin{pmatrix}
1(3)+(-2)(2) & 1(1)+(-2)(4) \\
0(3)+1(2) & 0(1)+1(4)
\end{pmatrix}
=
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}.
$$

**Verification**

$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
=
\begin{pmatrix}
1(-1)+2(2) & 1(-7)+2(4) \\
0(-1)+1(2) & 0(-7)+1(4)
\end{pmatrix}
=
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
=B.
$$

The check gives B, so X is correct. A⁻¹ must be multiplied on the left because A is on the left of X in the original equation.

---
