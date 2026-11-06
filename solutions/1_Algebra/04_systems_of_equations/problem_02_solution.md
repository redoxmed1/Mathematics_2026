### Exercise 2. Gaussian Elimination — One Solution

**Problem**

Solve the system using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

**Solution**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$

Apply the row operations:

$$
R_2 \leftarrow R_2-2R_1
$$

$$
R_3 \leftarrow R_3-R_1
$$

The result is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}
$$

Swap the second and third rows:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}
$$

Apply

$$
R_3 \leftarrow R_3+3R_2
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}
$$

Back substitution:

$$
-7z=-21
$$

Therefore,

$$
z=3
$$

The second row gives

$$
y-2(3)=-4
$$

Therefore,

$$
y=2
$$

The first row gives

$$
x+2+3=6
$$

Therefore,

$$
x=1
$$

The unique solution is

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
=
\begin{pmatrix}
1 \\
2 \\
3 \\
\end{pmatrix}
$$

**Check**

First equation:

$$
1+2+3=6
$$

Second equation:

$$
2(1)-2+3=3
$$

Third equation:

$$
1+2(2)-3=2
$$

All three equations are satisfied. Therefore, the solution is correct.
