### Exercise 8. Two Systems with the Same Coefficient Matrix

**Problem**

Solve both systems by elimination:

System 1:

$$
\begin{cases}
2x+y=5, \\
x-y=1.
\end{cases}
$$

System 2:

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the elimination steps and explain which calculations are the same.

**Solution**

**System 1**

The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}
$$

Swap the rows:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-2R_1
$$

We obtain

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3 \\
\end{pmatrix}
$$

Therefore,

$$
3y=3
$$

So

$$
y=1
$$

The first row gives

$$
x-1=1
$$

Therefore,

$$
x=2
$$

**System 2**

The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}
$$

Swap the rows:

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1 \\
\end{pmatrix}
$$

Apply the same operation:

$$
R_2 \leftarrow R_2-2R_1
$$

We obtain

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7 \\
\end{pmatrix}
$$

Therefore,

$$
3y=-7
$$

So

$$
y=-\frac{7}{3}
$$

The first row gives

$$
x+\frac{7}{3}=4
$$

Therefore,

$$
x=\frac{5}{3}
$$

**Comparison**

Both systems have the same coefficient matrix.

The row swap and elimination operations on the coefficient entries are identical. Only the right-hand side values change, producing different solutions.
