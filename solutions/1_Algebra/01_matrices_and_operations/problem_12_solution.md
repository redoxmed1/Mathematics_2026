### Exercise 12. Formula for a Matrix Power

**Problem**

Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}.
$$

Compute A², A³, and A⁴, and use them to formulate a conjecture for A^n. Then assume the formula is true for n, multiply by A, and explain why this gives the formula for n+1.

**Solution**

**1. Calculate the first powers**

$$
A^2=AA=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}.
$$

$$
A^3=A^2A=
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}.
$$

$$
A^4=A^3A=
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}.
$$

The top-right entry increases by 1 with each multiplication by A. This suggests the formula

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

for every nonnegative integer n.

**2. Induction step**

Assume the formula holds for some nonnegative integer n:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}.
$$

Multiply by A:

$$
A^{n+1}=A^nA=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & n+1 \\
0 & 1
\end{pmatrix}.
$$

This is exactly the proposed formula with n+1 in place of n. Since the formula also holds for n=0 because A⁰=I, mathematical induction proves it for all nonnegative integers n.

---
