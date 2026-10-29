### Exercise 15. Associativity of Multiplication and Different Calculation Paths

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
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix},
\qquad
C=
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix},
$$

compute (AB)C and A(BC). Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

**Solution**

The dimensions are compatible: A is 2× 3, B is 3× 2, and C is 2× 2. Therefore, AB and BC are both defined, and both final products have size 2× 2.

**1. Calculate (AB)C**

First calculate AB:

$$
AB=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
=
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}.
$$

Then multiply by C:

$$
(AB)C=
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}.
$$

**2. Calculate A(BC)**

First calculate BC:

$$
BC=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}.
$$

Then multiply A by BC:

$$
A(BC)=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}.
$$

Both calculation paths give the same result:

$$
(AB)C=A(BC)=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}.
$$

Each path requires two matrix multiplications, so both have two intermediate multiplication steps. Associativity means that changing the grouping of three compatible matrices does not change the final product. It does not mean that the order of the matrices can be changed.
