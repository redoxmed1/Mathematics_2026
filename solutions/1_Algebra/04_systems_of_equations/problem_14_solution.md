### Exercise 14. A Small Change in the Right-Hand Side

**Problem**

Compare the two systems.

System 1:

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.
\end{cases}
$$

System 2:

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1.
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

**Solution**

**System 1**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & 3 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-2R_1
$$

and

$$
R_3 \leftarrow R_3-3R_1
$$

The result is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & -3 \\
\end{pmatrix}
$$

The second row gives

$$
y=1
$$

The first row gives

$$
x=1
$$

The third row is consistent because

$$
3x=3
$$

Therefore, System 1 has exactly one solution:

$$
\begin{pmatrix}
x \\
y \\
\end{pmatrix}
=\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}
$$

**System 2**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & 3.1 \\
\end{pmatrix}
$$

Apply the same row operations:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & -2.9 \\
\end{pmatrix}
$$

Subtract the second row from the third row:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0.1 \\
\end{pmatrix}
$$

The last row represents

$$
0=0.1
$$

This is impossible.

Therefore, System 2 has no solution.

**Explanation**

The first two equations determine

$$
x=1
$$

and

$$
y=1
$$

These values require

$$
3x=3
$$

Changing the right-hand side to $3.1$ makes the third equation incompatible with the first two equations.

Thus, even a small change can turn a consistent system into an inconsistent one.
