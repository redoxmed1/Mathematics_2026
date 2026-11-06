# Exercise 2 – Addition and Scalar Multiplication

## Problem

For

$$
A = \begin{pmatrix} 1 & 2 \\ -1 & 3 \end{pmatrix}
$$

$$
B = \begin{pmatrix} 4 & -2 \\ 0 & 5 \end{pmatrix}
$$

compute $A + B$, $A - B$, and $3A - 2B$. Explain why matrix addition is possible only for matrices of the same size.

---

## Solution

Both matrices have size $2 \times 2$, so their corresponding entries can be added and subtracted directly.

### Step 1: Addition ($A + B$)

Add entries in matching positions:

$$
A + B = \begin{pmatrix} 1 + 4 & 2 + (-2) \\ -1 + 0 & 3 + 5 \end{pmatrix}
$$

$$
A + B = \begin{pmatrix} 5 & 0 \\ -1 & 8 \end{pmatrix}
$$

---

### Step 2: Subtraction ($A - B$)

Subtract entries in matching positions:

$$
A - B = \begin{pmatrix} 1 - 4 & 2 - (-2) \\ -1 - 0 & 3 - 5 \end{pmatrix}
$$

$$
A - B = \begin{pmatrix} -3 & 4 \\ -1 & -2 \end{pmatrix}
$$

---

### Step 3: Scalar multiplication and linear combination ($3A - 2B$)

First, compute scalar multiplication for $3A$:

$$
3A = \begin{pmatrix} 3(1) & 3(2) \\ 3(-1) & 3(3) \end{pmatrix}
$$

$$
3A = \begin{pmatrix} 3 & 6 \\ -3 & 9 \end{pmatrix}
$$

Next, compute scalar multiplication for $2B$:

$$
2B = \begin{pmatrix} 2(4) & 2(-2) \\ 2(0) & 2(5) \end{pmatrix}
$$

$$
2B = \begin{pmatrix} 8 & -4 \\ 0 & 10 \end{pmatrix}
$$

Now subtract the resulting matrices entry by entry:

$$
3A - 2B = \begin{pmatrix} 3 - 8 & 6 - (-4) \\ -3 - 0 & 9 - 10 \end{pmatrix}
$$

$$
3A - 2B = \begin{pmatrix} -5 & 10 \\ -3 & -1 \end{pmatrix}
$$

---

### Step 4: Explanation of size compatibility

Matrix addition and subtraction require both matrices to have the exact same number of rows and columns (the same dimensions) because every entry in one matrix must have a corresponding entry in the other matrix to be combined. 

Since both $A$ and $B$ are $2 \times 2$ matrices, all operations performed here are valid.

---

## Conclusion

- **Addition:** 

$$
A + B = \begin{pmatrix} 5 & 0 \\ -1 & 8 \end{pmatrix}
$$

- **Subtraction:** 

$$
A - B = \begin{pmatrix} -3 & 4 \\ -1 & -2 \end{pmatrix}
$$

- **Scalar combination:** 

$$
3A - 2B = \begin{pmatrix} -5 & 10 \\ -3 & -1 \end{pmatrix}
$$

- Matrix addition and subtraction are strictly restricted to matrices of identical dimensions so that entry-by-entry correspondence is preserved.
