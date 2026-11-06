### Exercise 13. Does Every Equation Add New Information?

**Problem**

Consider the system:

$$
\begin{cases}
x_1+x_2=10, \\
x_2+x_3=8, \\
x_1-x_3=2.
\end{cases}
$$

Solve it and check whether all three equations are independently necessary. If one follows from the others, show this by calculation.

**Solution**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
1 & 0 & -1 & \mid & 2 \\
\end{pmatrix}
$$

Apply

$$
R_3 \leftarrow R_3-R_1+R_2
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The last row is a zero row, so the third equation adds no new information.

Indeed, subtracting the second original equation from the first gives

$$
(x_1+x_2)-(x_2+x_3)=10-8
$$

which simplifies to

$$
x_1-x_3=2
$$

This is exactly the third equation.

Let

$$
x_2=t
$$

The first equation gives

$$
x_1=10-t
$$

The second equation gives

$$
x_3=8-t
$$

The complete solution is

$$
\begin{pmatrix}
x_1 \\
x_2 \\
x_3 \\
\end{pmatrix}
=
\begin{pmatrix}
10-t \\
t \\
8-t \\
\end{pmatrix}
$$

where

$$
t\in\mathbb{R}
$$

The third equation is redundant because it follows from the first two.
