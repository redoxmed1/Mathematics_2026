### Exercise 5. Matrix Times Vector

**Problem**

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix},
\qquad
x=
\begin{pmatrix}
4 \\
2
\end{pmatrix}.
$$

Compute Ax. Then express Ax as a linear combination of the columns of A, with coefficients coming from the vector x.

**Solution**

**1. Multiply the matrix by the vector**

Multiply each row of A by the column vector x:

$$
Ax=
\begin{pmatrix}
2(4)+(-1)(2) \\
1(4)+3(2)
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10
\end{pmatrix}.
$$

**2. Express the result using the columns**

Let the first and second columns of A be

$$
a_1=
\begin{pmatrix}
2 \\
1
\end{pmatrix},
\qquad
a_2=
\begin{pmatrix}
-1 \\
3
\end{pmatrix}.
$$

The entries of x are 4 and 2, so the matrix-vector product is the linear combination 4a_1+2a_2:

$$
Ax=
4\begin{pmatrix}2\\1\end{pmatrix}
+
2\begin{pmatrix}-1\\3\end{pmatrix}
=
\begin{pmatrix}8\\4\end{pmatrix}
+
\begin{pmatrix}-2\\6\end{pmatrix}
=
\begin{pmatrix}6\\10\end{pmatrix}.
$$

This agrees with the direct multiplication, verifying the result.

---
