### Exercise 2. Determinant of a 3×3 Matrix

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{pmatrix}
$$

compute the determinant using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

**Solution**

For Sarrus' rule, add the products of the three diagonals moving down to the right, and subtract the products of the three diagonals moving up to the right.

The positive diagonal products are

$$
1(3)(5)=15,
\qquad
2(4)(2)=16,
\qquad
(-1)(0)(1)=0.
$$

Their sum is

$$
15+16+0=31.
$$

The negative diagonal products are

$$
(-1)(3)(2)=-6,
\qquad
2(0)(5)=0,
\qquad
1(4)(1)=4.
$$

Their sum is

$$
-6+0+4=-2.
$$

Therefore,

$$
\det A=31-(-2)=33.
$$

**Check using a row operation**

Replace the third row by the third row minus twice the first row:

$$
R_3\leftarrow R_3-2R_1.
$$

Adding a multiple of one row to another row does not change the determinant. The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}.
$$

Expanding along the first column gives

$$
\det A
=1
\begin{vmatrix}
3 & 4 \\
-3 & 7
\end{vmatrix}
=1(3(7)-4(-3))
=21+12
=33.
$$

The check agrees with Sarrus' rule.

---
