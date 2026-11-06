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
AX=b
$$

Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row corresponds to one equation.

**Solution**

First, we identify the coefficients of the three variables in each equation.

The first equation is

$$
2x-y+z=4
$$

The second equation is

$$
x+3y-2z=1
$$

The third equation is

$$
3x+y+z=7
$$

**1. Coefficient Matrix**

The coefficient matrix contains the coefficients of the variables in the same order as they appear in the equations.

Therefore,

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}
$$

**2. Vector of Unknowns**

The vector of unknowns contains the variables of the system.

$$
X=
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
$$

**3. Right-Hand Side Vector**

The right-hand side vector contains the constant values from each equation.

$$
b=
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}
$$

**4. Matrix Representation**

The original system can now be written in the form

$$
AX=b
$$

Substituting the three components gives

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

**5. Explanation**

Each row of the coefficient matrix represents one equation.

- The first row contains the coefficients of the first equation: 2, -1, and 1.
- The second row contains the coefficients of the second equation: 1, 3, and -2.
- The third row contains the coefficients of the third equation: 3, 1, and 1.

The columns represent the variables in the same order: x, y, and z.

Therefore, the matrix representation contains exactly the same information as the original system.

**Final Result**

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}
$$

$$
X=
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
$$

$$
b=
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}
$$
