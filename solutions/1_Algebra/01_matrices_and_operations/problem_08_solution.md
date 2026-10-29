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

1. R_2arrow R_2-2R_1,
2. R_3arrow R_3+R_1,
3. interchange R_2 and R_3.

Write the matrix after each step. For each operation, state an operation that reverses it.

**Solution**

**Initial matrix**

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}.
$$

**Step 1: R_2arrow R_2-2R_1**

The new second row is

$$
(2,4,1)-2(1,2,-1)=(0,0,3).
$$

Therefore, the matrix becomes

$$
A_1=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}.
$$

The reverse operation is R_2arrow R_2+2R_1.

**Step 2: R_3arrow R_3+R_1**

Using the current first and third rows,

$$
(-1,1,3)+(1,2,-1)=(0,3,2).
$$

The matrix becomes

$$
A_2=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}.
$$

The reverse operation is R_3arrow R_3-R_1.

**Step 3: interchange R_2 and R_3**

Swap the second and third rows:

$$
A_3=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}.
$$

The reverse operation is to interchange R_2 and R_3 again. Each operation is reversible because adding back the subtracted row multiple, subtracting the added row, or swapping the same two rows restores the preceding matrix.

---
