### Exercise 4. Infinitely Many Solutions

**Problem**

Solve the system:

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and check one chosen parameter value.

**Solution**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
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

This gives

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$

The third row gives

$$
y=1
$$

The first row gives

$$
x+1+z=2
$$

Therefore,

$$
x+z=1
$$

The variable $z$ is free. Let

$$
z=t
$$

Then

$$
x=1-t
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
1-t \\
1 \\
t \\
\end{pmatrix}
$$

where

$$
t\in\mathbb{R}
$$

**Check**

Choose

$$
t=0
$$

The resulting point is

$$
(x,y,z)=(1,1,0)
$$

Substitute into the original equations:

$$
1+1+0=2
$$

$$
2(1)+2(1)+2(0)=4
$$

$$
1-1+0=0
$$

All three equations are satisfied.

Therefore, the system has infinitely many solutions.
