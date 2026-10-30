### Exercise 6. Transpose

**Problem**

For

$$
A=\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix},\qquad
B=\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}.
$$

Compute Aᵀ, Bᵀ, and AB. Then verify that (AB)ᵀ = BᵀAᵀ.

**Solution**

The transpose exchanges rows and columns.

$$
A^T=\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix},\qquad
B^T=\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}.
$$

**Calculate AB row by column.**

$$
AB=\begin{pmatrix}
1(1)+2(2)+3(-1) & 1(0)+2(1)+3(3) \\
4(1)+5(2)+6(-1) & 4(0)+5(1)+6(3)
\end{pmatrix}
=\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}.
$$

Therefore,

$$
(AB)^T=\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}.
$$

**Independently calculate BᵀAᵀ row by column.** The first row is found from the dot products

$$
1(1)+2(2)+(-1)(3)=2,\qquad
1(4)+2(5)+(-1)(6)=8.
$$

The second row is found from

$$
0(1)+1(2)+3(3)=11,\qquad
0(4)+1(5)+3(6)=23.
$$

Thus,

$$
B^TA^T=\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}=(AB)^T.
$$

The independent row-by-column calculations verify that transposing a product reverses the order of its factors.
