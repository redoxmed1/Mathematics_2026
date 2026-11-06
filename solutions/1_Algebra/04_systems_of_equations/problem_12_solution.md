### Exercise 12. Homogeneous System

**Problem**

Solve the homogeneous system:

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why the zero vector always satisfies a homogeneous system.

**Solution**

The augmented matrix is

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
2 & 4 & -2 & \mid & 0 \\
1 & -1 & 2 & \mid & 0 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-2R_1
$$

and

$$
R_3 \leftarrow R_3-R_1
$$

The result is

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
\end{pmatrix}
$$

The third row gives

$$
-3y+3z=0
$$

Therefore,

$$
y=z
$$

Let

$$
y=t
$$

Then

$$
z=t
$$

Substitute into the first equation:

$$
x+2t-t=0
$$

Therefore,

$$
x=-t
$$

The complete solution is

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
=
\begin{pmatrix}
-t \\
t \\
t \\
\end{pmatrix}
$$

where

$$
t\in\mathbb{R}
$$

A homogeneous system has zero on the right-hand side of every equation.

Substituting zero for all variables makes every left-hand side equal to zero.

Therefore, the zero vector always satisfies a homogeneous system.
