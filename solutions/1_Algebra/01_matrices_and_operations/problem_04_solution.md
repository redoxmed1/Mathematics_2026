### Exercise 4. Matrix multiplication is not commutative

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2 & 0 \\
3 & 1
\end{pmatrix},
$$

calculate \(AB\) and \(BA\). Use the results to determine whether matrix multiplication is commutative for these matrices.

## Solution

To multiply matrices, each product entry is the dot product of a row of the first matrix with a column of the second matrix.

### 1. Calculate \(AB\)

$$
AB=
\begin{pmatrix}
1(2)+2(3) & 1(0)+2(1) \\
0(2)+1(3) & 0(0)+1(1)
\end{pmatrix}
=
\begin{pmatrix}
8 & 2 \\
3 & 1
\end{pmatrix}.
$$

For example, the top-left entry is the first row of \(A\) dotted with the first column of \(B\): \(1(2)+2(3)=8\).

### 2. Calculate \(BA\)

Reversing the order means taking rows of \(B\) dotted with columns of \(A\):

$$
BA=
\begin{pmatrix}
2(1)+0(0) & 2(2)+0(1) \\
3(1)+1(0) & 3(2)+1(1)
\end{pmatrix}
=
\begin{pmatrix}
2 & 4 \\
3 & 7
\end{pmatrix}.
$$

The corresponding entries differ; for example, the top-left entries are \(8\) in \(AB\) and \(2\) in \(BA\). Therefore,

$$
AB\ne BA.
$$

This example shows that matrix multiplication is not commutative in general: changing the order of the factors can change the product.
