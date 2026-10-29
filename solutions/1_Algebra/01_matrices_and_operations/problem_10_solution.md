### Exercise 10. Columns of a Matrix Product

**Problem**

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix},
$$

denote the columns of B by b_1 and b_2.

1. Compute Ab_1 and Ab_2.
2. Compute the matrix AB.
3. Compare the results and explain why the columns of AB are exactly the vectors Ab_1 and Ab_2.

**Solution**

The columns of B are

$$
b_1=
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix},
\qquad
b_2=
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}.
$$

**1. Compute Ab_1**

$$
Ab_1=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix}
=
\begin{pmatrix}
1-2+0 \\
0-1+3
\end{pmatrix}
=
\begin{pmatrix}
-1 \\
2
\end{pmatrix}.
$$

**Compute Ab_2**

$$
Ab_2=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}
=
\begin{pmatrix}
2+0+0 \\
0+0+1
\end{pmatrix}
=
\begin{pmatrix}
2 \\
1
\end{pmatrix}.
$$

**2. Compute AB**

$$
AB=
\begin{pmatrix}
1(1)+2(-1)+0(3) & 1(2)+2(0)+0(1) \\
0(1)+1(-1)+1(3) & 0(2)+1(0)+1(1)
\end{pmatrix}
=
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}.
$$

**3. Compare the columns**

The first column of AB is (-1,2)ᵀ=Ab_1, and the second column is (2,1)ᵀ=Ab_2. Matrix multiplication applies A to each column of B separately; therefore, the columns of AB are precisely Ab_1 and Ab_2.

---
