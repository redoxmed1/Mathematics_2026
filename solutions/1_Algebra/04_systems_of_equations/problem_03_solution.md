### Exercise 3. Inconsistent System

**Problem**

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

**Solution**

The augmented matrix is

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-2R_1
$$

The matrix becomes

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row represents

$$
0x+0y=1
$$

This is impossible because zero cannot equal one.

Therefore, the system is inconsistent and has no solution.
