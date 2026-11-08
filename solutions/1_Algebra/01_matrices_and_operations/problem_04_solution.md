### Exercise 4. Matrix Multiplication and Noncommutativity

**Problem**

Given:

$$
A=\begin{pmatrix}
1&2\\
0&1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
2&0\\
3&1
\end{pmatrix}
$$

Compute AB and BA. Is AB = BA? Use this example to explain what noncommutativity of matrix multiplication means.

### Solution

**1. Calculate AB**

To calculate AB, we multiply each row of A by each column of B.

$$
AB=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
\begin{pmatrix}
2&0\\
3&1
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
1(2)+2(3)&1(0)+2(1)\\
0(2)+1(3)&0(0)+1(1)
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
8&2\\
3&1
\end{pmatrix}
$$

**2. Calculate BA**

Now we reverse the order of multiplication.

$$
BA=
\begin{pmatrix}
2&0\\
3&1
\end{pmatrix}
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
2(1)+0(0)&2(2)+0(1)\\
3(1)+1(0)&3(2)+1(1)
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
2&4\\
3&7
\end{pmatrix}
$$

**3. Compare AB and BA**

We obtained:

$$
AB=
\begin{pmatrix}
8&2\\
3&1
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
2&4\\
3&7
\end{pmatrix}
$$

Therefore:

$$
AB\neq BA
$$

**Conclusion**

Matrix multiplication is not commutative in general. This means that changing the order of multiplication can produce a different result.

In this example, AB is not equal to BA, which demonstrates the noncommutativity of matrix multiplication.
