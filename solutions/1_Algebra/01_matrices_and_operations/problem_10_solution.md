### Exercise 10. Columns of a Matrix Product

**Problem**

Given:

$$
A=\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
$$

Denote the columns of B by b₁ and b₂.

1. Compute Ab₁ and Ab₂.
2. Compute the matrix AB.
3. Compare the results and explain why the columns of AB are exactly the vectors Ab₁ and Ab₂.

### Solution

**1. Identify the columns of B**

The first column of B is:

$$
b_1=\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}
$$

The second column of B is:

$$
b_2=\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
$$

**2. Calculate Ab₁**

$$
Ab_1=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}
$$

Multiply each row of A by the column vector:

$$
Ab_1=
\begin{pmatrix}
1(1)+2(-1)+0(3)\\
0(1)+1(-1)+1(3)
\end{pmatrix}
$$

$$
Ab_1=
\begin{pmatrix}
1-2+0\\
0-1+3
\end{pmatrix}
$$

Therefore:

$$
Ab_1=
\begin{pmatrix}
-1\\
2
\end{pmatrix}
$$

**3. Calculate Ab₂**

$$
Ab_2=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
$$

$$
Ab_2=
\begin{pmatrix}
1(2)+2(0)+0(1)\\
0(2)+1(0)+1(1)
\end{pmatrix}
$$

$$
Ab_2=
\begin{pmatrix}
2+0+0\\
0+0+1
\end{pmatrix}
$$

Therefore:

$$
Ab_2=
\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

**4. Calculate the matrix AB**

We multiply A by B:

$$
AB=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
$$

Calculate each entry:

$$
AB=
\begin{pmatrix}
1(1)+2(-1)+0(3)&1(2)+2(0)+0(1)\\
0(1)+1(-1)+1(3)&0(2)+1(0)+1(1)
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
-1&2\\
2&1
\end{pmatrix}
$$

**5. Compare the results**

We calculated:

$$
Ab_1=
\begin{pmatrix}
-1\\
2
\end{pmatrix}
$$

$$
Ab_2=
\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

And:

$$
AB=
\begin{pmatrix}
-1&2\\
2&1
\end{pmatrix}
$$

The first column of AB is exactly Ab₁, and the second column is exactly Ab₂.

**Conclusion**

The columns of the product AB are obtained by multiplying A by each column of B separately.

Therefore, the matrix product AB is formed by placing the vectors Ab₁ and Ab₂ next to each other as columns. This confirms that matrix multiplication can be understood as
