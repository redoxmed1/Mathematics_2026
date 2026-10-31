
### Exercise 7. Inverse of a Product

**Problem**

Given the matrices

$$
A=\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
2 & 0\\
0 & 3
\end{pmatrix},
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain why the inverse of a product reverses the order of the factors.

**Solution**

**1. Calculate $AB$**

Multiply the rows of $A$ by the columns of $B$:

$$
AB=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0\\
0 & 3
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
1(2)+1(0) & 1(0)+1(3)\\
0(2)+1(0) & 0(0)+1(3)
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
2 & 3\\
0 & 3
\end{pmatrix}
$$

**2. Calculate $(AB)^{-1}$**

First calculate the determinant:

$$
\det(AB)=2(3)-3(0)=6
$$

Since the determinant is nonzero, the inverse exists.

Using the inverse formula for a $2\times2$ matrix:

$$
\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}^{-1}
=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b\\
-c & a
\end{pmatrix}
$$

Therefore:

$$
(AB)^{-1}
=
\frac{1}{6}
\begin{pmatrix}
3 & -3\\
0 & 2
\end{pmatrix}
$$

$$
(AB)^{-1}
=
\begin{pmatrix}
\frac12 & -\frac12\\
0 & \frac13
\end{pmatrix}
$$

**3. Calculate $A^{-1}$ and $B^{-1}$ separately**

For matrix $A$:

$$
\det(A)=1(1)-1(0)=1
$$

$$
A^{-1}
=
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
$$

For matrix $B$:

$$
\det(B)=2(3)-0(0)=6
$$

$$
B^{-1}
=
\begin{pmatrix}
\frac12 & 0\\
0 & \frac13
\end{pmatrix}
$$

**4. Calculate $B^{-1}A^{-1}$**

Multiply the inverses in the reversed order:

$$
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12 & 0\\
0 & \frac13
\end{pmatrix}
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
$$

Multiply rows by columns:

$$
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12(1)+0(0) &
\frac12(-1)+0(1)\\
0(1)+\frac13(0) &
0(-1)+\frac13(1)
\end{pmatrix}
$$

Simplifying:

$$
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12 & -\frac12\\
0 & \frac13
\end{pmatrix}
$$

Both methods give the same result:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

**5. Explanation of the reversed order**

When we calculate $ABx$, matrix $B$ acts on the vector $x$ first, and then matrix $A$ acts on the result.

To undo these operations, we must reverse their order.

First, we undo $A$ using $A^{-1}$. Then, we undo $B$ using $B^{-1}$.

Therefore:

$$
A^{-1}(ABx)=Bx
$$

$$
B^{-1}A^{-1}(ABx)=x
$$

This proves that:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

**Conclusion**

The inverse of a product reverses the order of the original matrices because the last transformation applied must be the first one undone. The calculations confirm that both methods produce the same inverse matrix.

