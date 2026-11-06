### Exercise. Matrix Times Vector

**Problem**

Let

$$
A = \begin{pmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{pmatrix},
\qquad
x = \begin{pmatrix} x_1 \\ x_2 \end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

**Solution**

**1. Multiply the matrix by the vector**

Multiply each row of $A$ by the column vector $x$:

$$
Ax = \begin{pmatrix} a_{11}(x_1) + a_{12}(x_2) \\ a_{21}(x_1) + a_{22}(x_2) \end{pmatrix} = \begin{pmatrix} \text{result}_1 \\ \text{result}_2 \end{pmatrix}
$$

**2. Express the result using the columns**

Let the first and second columns of $A$ be

$$
a_1 = \begin{pmatrix} a_{11} \\ a_{21} \end{pmatrix},
\qquad
a_2 = \begin{pmatrix} a_{12} \\ a_{22} \end{pmatrix}.
$$

The entries of $x$ are $x_1$ and $x_2$, so the matrix-vector product is the linear combination $x_1 a_1 + x_2 a_2$:

$$
Ax = x_1 \begin{pmatrix} a_{11} \\ a_{21} \end{pmatrix} + x_2 \begin{pmatrix} a_{12} \\ a_{22} \end{pmatrix} = \begin{pmatrix} \text{term}_1 \\ \text{term}_2 \end{pmatrix} + \begin{pmatrix} \text{term}_3 \\ \text{term}_4 \end{pmatrix} = \begin{pmatrix} \text{result}_1 \\ \text{result}_2 \end{pmatrix}
$$

This agrees with the direct multiplication, verifying the result.
