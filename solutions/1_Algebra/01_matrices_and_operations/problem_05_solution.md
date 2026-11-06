# Exercise 5 – Matrix Times Vector

## Problem

Let

$$
A = \left(\begin{array}{rr} 2 & -1 \\ 1 & 3 \end{array}\right)
$$

and

$$
x = \left(\begin{array}{r} 4 \\ 2 \end{array}\right)
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

---

## Solution

### Step 1: Multiply the matrix by the vector

Multiply each row of $A$ by the column vector $x$:

$$
Ax = \left(\begin{array}{rr} 2 & -1 \\ 1 & 3 \end{array}\right) \left(\begin{array}{r} 4 \\ 2 \end{array}\right)
$$

Compute the entries:

$$
Ax = \left(\begin{array}{r} (2)(4) + (-1)(2) \\ (1)(4) + (3)(2) \end{array}\right)
$$

Simplify the arithmetic:

$$
Ax = \left(\begin{array}{r} 6 \\ 10 \end{array}\right)
$$

---

### Step 2: Express the result using the columns

Let the first and second columns of $A$ be denoted as $a_1$ and $a_2$:

$$
a_1 = \left(\begin{array}{r} 2 \\ 1 \end{array}\right), \quad a_2 = \left(\begin{array}{r} -1 \\ 3 \end{array}\right)
$$

The entries of $x$ are $4$ and $2$, so the matrix-vector product can be written as the linear combination $4a_1 + 2a_2$:

$$
Ax = 4 \left(\begin{array}{r} 2 \\ 1 \end{array}\right) + 2 \left(\begin{array}{r} -1 \\ 3 \end{array}\right)
$$

Perform the scalar multiplications:

$$
Ax = \left(\begin{array}{r} 8 \\ 4 \end{array}\right) + \left(\begin{array}{r} -2 \\ 6 \end{array}\right)
$$

Add the vectors entry by entry:

$$
Ax = \left(\begin{array}{r} 6 \\ 10 \end{array}\right)
$$

---

## Conclusion

- The direct matrix-vector product is:

$$
Ax = \left(\begin{array}{r} 6 \\ 10 \end{array}\right)
$$

- Expressed as a linear combination of the columns of $A$ using the components of $x$:

$$
4 \left(\begin{array}{r} 2 \\ 1 \end{array}\right) + 2 \left(\begin{array}{r} -1 \\ 3 \end{array}\right) = \left(\begin{array}{r} 6 \\ 10 \end{array}\right)
$$

This verifies that multiplying a matrix by a vector yields a linear combination of its columns.
