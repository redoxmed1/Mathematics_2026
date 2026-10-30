### Exercise 7. Inverse of a Product

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix},
$$

compute (AB)⁻¹ and B⁻¹A⁻¹. Check that the results are the same and explain the meaning of the reversed order.

**Solution**

First calculate AB:

$$
AB=
\begin{pmatrix}
1(2)+1(0) & 1(0)+1(3) \\
0(2)+1(0) & 0(0)+1(3)
\end{pmatrix}
=
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}.
$$

The determinant is 2(3) − 3(0) = 6. Thus,

$$
(AB)^{-1}
=\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13
\end{pmatrix}.
$$

Now calculate the inverses separately:

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix},
\qquad
B^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13
\end{pmatrix}.
$$

Multiply them in the reversed order:

$$
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12(1)+0(0) &
\frac12(-1)+0(1) \\
0(1)+\frac13(0) &
0(-1)+\frac13(1)
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13
\end{pmatrix}.
$$

Therefore,

$$
(AB)^{-1}=B^{-1}A^{-1}.
$$

The order is reversed because to undo the operation AB, the transformation B is undone first and then A. In general, the inverse of a product reverses the order of the factors.

---
