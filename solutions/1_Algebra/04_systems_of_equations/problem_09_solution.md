### Exercise 9. A System from a Sum Condition

**Problem**

Find numbers $x$ and $y$ satisfying

$$
x+y=10
$$

$$
2x+5y=32
$$

Solve the system and explain geometrically why the solution is unique.

**Solution**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
2 & 5 & \mid & 32 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-2R_1
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
0 & 3 & \mid & 12 \\
\end{pmatrix}
$$

The second row gives

$$
3y=12
$$

Therefore,

$$
y=4
$$

The first equation gives

$$
x+4=10
$$

Therefore,

$$
x=6
$$

The solution is

$$
\begin{pmatrix}
x \\
y \\
\end{pmatrix}
=\begin{pmatrix}
6 \\
4 \\
\end{pmatrix}
$$

**Geometric explanation**

Each equation represents a straight line in the plane.

The two lines have different slopes, so they intersect at exactly one point.

Their intersection is

$$
(6,4)
$$

Therefore, the solution is unique.
