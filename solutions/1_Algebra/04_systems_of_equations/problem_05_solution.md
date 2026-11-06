### Exercise 5. Row Echelon Form and Number of Solutions

**Problem**

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

**Solution**

The augmented matrix is already in row echelon form.

The corresponding equations are

$$
x+2y-z=3
$$

$$
y+2z=1
$$

The last row gives no additional condition.

The pivot columns are the first and second columns. Therefore, $z$ is a free variable.

Let

$$
z=t
$$

From the second equation,

$$
y+2t=1
$$

Therefore,

$$
y=1-2t
$$

Substitute into the first equation:

$$
x+2(1-2t)-t=3
$$

Therefore,

$$
x=1+5t
$$

The solution is

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
=\begin{pmatrix}
1+5t \\
1-2t \\
t \\
\end{pmatrix}
$$

where

$$
t\in\mathbb{R}
$$

There is one free variable, so the system has infinitely many solutions.
