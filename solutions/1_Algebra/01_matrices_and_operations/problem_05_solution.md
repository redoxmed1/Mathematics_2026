# Exercise 5 – Matrix Times Vector

## Problem

Let

$$
A = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix}
$$

and

$$
x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

---

## Solution

### Step 1: Multiply the matrix by the vector

Multiply each row of $A$ by the column vector $x$:

$$
Ax = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix} \begin{pmatrix} 4 \\ 2 \end{pmatrix}
$$

Compute the entries:

$$
Ax = \begin{pmatrix} (2)(4) + (-1)(2) \\ (1)(4) + (3)(2) \end{pmatrix}
$$

Simplify the arithmetic:

$$
Ax = \begin{pmatrix} 6 \\ 10 \end{pmatrix}
$$

---

### Step 2: Express the result using the columns

Let the first and second columns of $A$ be denoted as $a_1$ and $a_2$:

$$
a_1 = \begin{pmatrix} 2 \\ 1 \end{pmatrix}, \quad a_2 = \begin{pmatrix} -1 \\ 3 \end{pmatrix}
$$

The entries of $x$ are $4$ and $2$, so the matrix-vector product can be written as the linear combination $4a_1 + 2a_2$:

$$
Ax = 4 \begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2 \begin{pmatrix} -1 \\ 3 \end{pmatrix}
$$

Perform the scalar multiplications:

$$
Ax = \begin{pmatrix} 8 \\ 4 \end{pmatrix} + \begin{pmatrix} -2 \\ 6 \end{pmatrix}
$$

Add the vectors entry by entry:

$$
Ax = \begin{pmatrix} 6 \\ 10 \end{pmatrix}
$$

---

## Conclusion

- The direct matrix-vector product is:

$$
Ax = \begin{pmatrix} 6 \\ 10 \end{pmatrix}
$$

- Expressed as a linear combination of the columns of $A$ using the components of $x$:

$$
4 \begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2 \begin{pmatrix} -1 \\ 3 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}
$$

This verifies that multiplying a matrix by a vector yields a linear combination of its columns.
