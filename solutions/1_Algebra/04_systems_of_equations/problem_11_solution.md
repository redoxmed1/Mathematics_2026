### Exercise 11. A Parameter in a System of Three Equations

**Problem**

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and analyze the parameter values for which a calculation step ceases to be valid.

**Solution**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
1 & t & 1 & \mid & 2 \\
1 & 1 & t & \mid & 3 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-R_1
$$

and

$$
R_3 \leftarrow R_3-R_1
$$

The result is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t-1 & 0 & \mid & 1 \\
0 & 0 & t-1 & \mid & 2 \\
\end{pmatrix}
$$

**Case 1:**

If

$$
t\neq1
$$

The second row gives

$$
(t-1)y=1
$$

Therefore,

$$
y=\frac{1}{t-1}
$$

The third row gives

$$
(t-1)z=2
$$

Therefore,

$$
z=\frac{2}{t-1}
$$

The first equation gives

$$
x=1-\frac{3}{t-1}
$$

There is exactly one solution:

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
=\begin{pmatrix}
1-\frac{3}{t-1} \\
\frac{1}{t-1} \\
\frac{2}{t-1} \\
\end{pmatrix}
$$

**Case 2:**

If

$$
t=1
$$

The reduced matrix becomes

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & 0 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 2 \\
\end{pmatrix}
$$

The second and third rows represent contradictions.

Therefore, the system has no solution.

**Conclusion**

- Exactly one solution if $t\neq1$.
- No solution if $t=1$.
- Infinitely many solutions never occur.
