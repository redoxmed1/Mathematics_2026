### Exercise 6. A System with a Parameter — Which Cases Actually Occur?

**Problem**

Analyze the system depending on the parameter $a$:

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Determine which possibilities occur: exactly one solution, infinitely many solutions, or no solution.

**Solution**

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}
$$

Apply

$$
R_2 \leftarrow R_2-aR_1
$$

The result is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}
$$

**Case 1:**

If

$$
a=2
$$

the second row becomes a zero row.

Both equations describe the same condition:

$$
x+y=2
$$

Therefore, there are infinitely many solutions.

**Case 2:**

If

$$
a\neq2
$$

the second row represents

$$
0=4-2a
$$

This is a contradiction.

Therefore, there is no solution.

**Conclusion**

- If $a=2$, infinitely many solutions.
- If $a\neq2$, no solution.
- Exactly one solution never occurs because the coefficient rows are always proportional.
