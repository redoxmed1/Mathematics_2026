### Exercise 8. Row Operations and Their Reversibility

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix},
$$

perform, in order:

1. R₂ → R₂ − 2R₁
2. R₃ → R₃ + R₁
3. Interchange R₂ and R₃.

Write the matrix after each step. Then, for each operation,
state an operation that reverses it.

**Solution**

**Initial matrix**

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
$$

**Step 1: R₂ → R₂ − 2R₁**

Replace the second row by the second row minus twice
the first row.

$$
R_2=(2,4,1)-2(1,2,-1)
$$

$$
R_2=(0,0,3)
$$

The resulting matrix is

$$
A_1=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
$$

The reverse operation is:

R₂ → R₂ + 2R₁

**Step 2: R₃ → R₃ + R₁**

Replace the third row by the third row plus the first row.

$$
R_3=(-1,1,3)+(1,2,-1)
$$

$$
R_3=(0,3,2)
$$

The resulting matrix is

$$
A_2=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
$$

The reverse operation is:

R₃ → R₃ − R₁

**Step 3: Interchange R₂ and R₃**

Swap the second and third rows.

$$
A_3=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
$$

The reverse operation is to interchange R₂ and R₃ again.

**Conclusion**

Each row operation is reversible.

- Subtracting twice the first row is reversed by adding twice the first row.
- Adding the first row is reversed by subtracting the first row.
- Swapping two rows is reversed by performing the same swap again.

These operations demonstrate that elementary row operations
are controlled and reversible transformations of a matrix.
