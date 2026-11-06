### Exercise 1. From a System to a Matrix

**Problem**

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7
\end{cases}
$$

in the form

$$
Ax=b
$$

Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row corresponds to one equation.

**Solution**

The coefficient matrix is

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}
$$

The vector of unknowns is

$$
X=
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
$$

The right-hand side vector is

$$
b=
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}
$$

Therefore, the system can be written as

$$
AX=b
$$

or

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
=
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}
$$

Each row of the coefficient matrix contains the coefficients of one equation.

- The first row represents the first equation.
- The second row represents the second equation.
- The third row represents the third equation.

Therefore, the matrix representation contains exactly the same information as the original system.
