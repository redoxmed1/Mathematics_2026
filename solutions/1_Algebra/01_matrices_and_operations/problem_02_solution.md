### Exercise 2. Addition and Scalar Multiplication

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
4 & -2 \\
0 & 5
\end{pmatrix},
$$

compute A+B, A-B, and 3A-2B. Explain why matrix addition is possible only for matrices of the same size.

**Solution**

Both matrices have size 2× 2, so their corresponding entries can be added and subtracted.

**1. Addition**

Add entries in matching positions:

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5
\end{pmatrix}
=
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}.
$$

**2. Subtraction**

Subtract entries in matching positions:

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5
\end{pmatrix}
=
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}.
$$

**3. Scalar multiplication before subtraction**

First calculate 3A:

$$
3A=
\begin{pmatrix}
3(1) & 3(2) \\
3(-1) & 3(3)
\end{pmatrix}
=
\begin{pmatrix}
3 & 6 \\
-3 & 9
\end{pmatrix}.
$$

Then calculate 2B:

$$
2B=
\begin{pmatrix}
2(4) & 2(-2) \\
2(0) & 2(5)
\end{pmatrix}
=
\begin{pmatrix}
8 & -4 \\
0 & 10
\end{pmatrix}.
$$

Now subtract the two matrices entry by entry:

$$
3A-2B=
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10
\end{pmatrix}
=
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}.
$$

Matrix addition and subtraction require the same number of rows and columns because each entry must have a corresponding entry in the other matrix. Here, all operations are valid because both matrices are 2× 2.

---
