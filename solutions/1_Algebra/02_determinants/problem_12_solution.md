### Exercise 12. A Parameter Revealed by a Row Operation

**Problem**

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
$$

find the values of t for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2\leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter found.

**Solution**

Apply the required row operation:

$$
R_2\leftarrow R_2-2R_1.
$$

This operation does not change the determinant. The new second row is

$$
(2,4,t)-2(1,2,3)=(0,0,t-6).
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1
\end{pmatrix}.
$$

Expand along the first column, which contains two zeros below its first entry:

$$
\begin{aligned}
\det A(t)
&=
\begin{vmatrix}
0 & t-6 \\
1 & 1
\end{vmatrix}
\\
&=0(1)-(t-6)(1)
\\
&=6-t.
\end{aligned}
$$

The matrix is not invertible when its determinant is zero:

$$
6-t=0.
$$

Therefore,

$$
t=6.
$$

When t = 6, the original second row is

$$
(2,4,6)=2(1,2,3),
$$

so the second row is twice the first row. The rows are linearly dependent, which explains why the determinant is zero.

---
