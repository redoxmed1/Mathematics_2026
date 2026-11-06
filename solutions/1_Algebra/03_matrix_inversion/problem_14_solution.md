# Exercise 14 – A Matrix That Is Its Own Inverse

## Problem

Assume that a square matrix $A$ satisfies $A^2 = I$. Show that $A^{-1} = A$. Then give an example of a $2 \times 2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

---

## Solution

### Step 1: Prove that A⁻¹ = A

The condition $A^2 = I$ can be written by definition of matrix powers as:

$$
AA = I
$$

By the definition of a matrix inverse, if a matrix multiplied by $A$ yields the identity matrix $I$, that matrix is the inverse of $A$. 

Since multiplying $A$ by itself ($AA = I$) produces the identity matrix, $A$ serves as its own inverse:

$$
A^{-1} = A
$$

---

### Step 2: Construct an example matrix different from I and -I

Choose the following $2 \times 2$ permutation matrix:

$$
A = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}
$$

This matrix is clearly different from both the identity matrix $I$ and its negative $-I$.

---

### Step 3: Verify the condition by multiplication

Calculate the square of matrix $A$ by multiplying it by itself:

$$
A^2 = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}
$$

Compute each entry via row-by-row multiplication:

$$
A^2 = \begin{pmatrix} (0)(0) + (1)(1) & (0)(1) + (1)(0) \\ (1)(0) + (0)(1) & (1)(1) + (0)(0) \end{pmatrix}
$$

Simplify the arithmetic:

$$
A^2 = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = I
$$

Since $A^2 = I$, the matrix satisfies the given condition, confirming that $A^{-1} = A$.

---

## Conclusion

- If $A^2 = I$, then $A^{-1} = A$ because multiplying $A$ by itself yields the identity matrix.
- The example matrix:

$$
A = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}
$$

satisfies $A^2 = I$ and is distinct from $I$ and $-I$.
- Thus, its inverse is itself:

$$
A^{-1} = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}
$$
