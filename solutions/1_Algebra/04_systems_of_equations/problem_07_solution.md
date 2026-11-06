### Exercise 7. Choosing a Method Deliberately

**Problem**

Choose the best method for each situation and justify your choice.

1. One system with a triangular coefficient matrix.
2. Three systems with the same invertible matrix, when the inverse is already known.
3. One 3x3 system where the inverse is not given and only one solution vector is required.

For case 1, solve completely. For cases 2 and 3, describe the method.

**Solution**

**Case 1: Triangular coefficient matrix**

The system is

$$
\begin{cases}
2x-y=3, \\
4y=8.
\end{cases}
$$

Back substitution is the simplest method.

The second equation gives

$$
4y=8
$$

Therefore,

$$
y=2
$$

Substitute into the first equation:

$$
2x-2=3
$$

Therefore,

$$
2x=5
$$

and

$$
x=\frac{5}{2}
$$

The solution is

$$
\begin{pmatrix}
x \\
y \\
\end{pmatrix}
=
\begin{pmatrix}
\frac{5}{2} \\
2 \\
\end{pmatrix}
$$

**Case 2: Three systems with the same invertible matrix**

For the systems

$$
Ax=b_1
$$

$$
Ax=b_2
$$

$$
Ax=b_3
$$

when the inverse is already known, use

$$
x_1=A^{-1}b_1
$$

$$
x_2=A^{-1}b_2
$$

$$
x_3=A^{-1}b_3
$$

The inverse matrix is calculated only once and reused for all three systems.

**Case 3: One system with an unknown inverse**

Gaussian elimination is suitable because only one solution vector is required.

Calculating the full inverse matrix would require extra work that is unnecessary.
