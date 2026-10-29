### Exercise 6. Transpose

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix},
$$

compute Aᵀ, Bᵀ, and AB. Then verify that (AB)ᵀ=BᵀAᵀ.

**Solution**

The transpose exchanges rows and columns.

**1. Transpose of A**

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}.
$$

**2. Transpose of B**

$$
B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}.
$$

**3. Calculate AB**

The product is defined because A is 2× 3 and B is 3× 2. The result has size 2× 2.

$$
AB=
\begin{pmatrix}
1(1)+2(2)+3(-1) & 1(0)+2(1)+3(3) \\
4(1)+5(2)+6(-1) & 4(0)+5(1)+6(3)
\end{pmatrix}
=
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}.
$$

Therefore,

$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}.
$$

**4. Verify BᵀAᵀ**

Multiply Bᵀ (size 2× 3) by Aᵀ (size 3× 2):

$$
B^TA^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
=
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}.
$$

Thus,

$$
(AB)^T=B^TA^T.
$$

The order reverses when transposing a product: the transpose of AB is BᵀAᵀ.

---
