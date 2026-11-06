### Exercise 15. Classifying Three Systems

**Problem**

Classify each system as having one solution, infinitely many solutions, or no solution.

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0.
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4.
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5.
\end{cases}
$$

Justify each classification using elimination.

**Solution**

**System 1**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
1 & -1 & \mid & 0 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-R_1
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -2 & \mid & -2 \\
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

Therefore, the system has exactly one solution:

$$
\begin{pmatrix}
x \\
y \\
\end{pmatrix}
=
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}
$$

**System 2**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 4 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-2R_1
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The second equation is a multiple of the first, so it adds no new information.

Let

$$
y=t
$$

Then

$$
x=2-t
$$

The system has infinitely many solutions:

$$
\begin{pmatrix}
x \\
y \\
\end{pmatrix}
=
\begin{pmatrix}
2-t \\
t \\
\end{pmatrix}
$$

where

$$
t\in\mathbb{R}
$$

**System 3**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 5 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-2R_1
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row represents

$$
0=1
$$

This is a contradiction.

Therefore, the system has no solution.

**Final classification**

- System 1: exactly one solution.
- System 2: infinitely many solutions.
- System 3: no solution.
