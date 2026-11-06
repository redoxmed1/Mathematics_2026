# Exercise 12 – Finding Inverses Without Starting from Scratch

## Problem

It is known that:

$$A^{-1} = \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix}$$

Without finding matrix $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property of matrix inverses.

---

## Solution

### Step 1: Compute $(3A)^{-1}$ using the scalar property

#### Property
For any non-zero scalar $c$ and invertible matrix $A$:

$$(cA)^{-1} = \frac{1}{c} A^{-1}$$

#### Calculation
Apply the property for $c = 3$:

$$(3A)^{-1} = \frac{1}{3} \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix}$$

Multiply the scalar into each entry:

$$(3A)^{-1} = \begin{pmatrix} \frac{2}{3} & -\frac{1}{3} \\ -1 & \frac{2}{3} \end{pmatrix}$$

---

### Step 2: Compute $(A^T)^{-1}$ using the transpose property

#### Property
The inverse of the transpose of a matrix equals the transpose of its inverse:

$$(A^T)^{-1} = (A^{-1})^T$$

#### Calculation
Transpose the given matrix $A^{-1}$ by swapping its rows and columns:

$$(A^T)^{-1} = \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix}^T = \begin{pmatrix} 2 & -3 \\ -1 & 2 \end{pmatrix}$$

---

### Step 3: Compute $(A^2)^{-1}$ using the product property

#### Property
The inverse of a product of matrices is the product of their inverses in reverse order:

$$(AB)^{-1} = B^{-1} A^{-1}$$

For $A^2 = AA$, this gives:

$$(A^2)^{-1} = (AA)^{-1} = A^{-1} A^{-1} = (A^{-1})^2$$

#### Calculation
Multiply $A^{-1}$ by itself:

$$(A^2)^{-1} = \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix} \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix}$$

Calculate each entry via row-by-column matrix multiplication:

$$(A^2)^{-1} = \begin{pmatrix} (2)(2) + (-1)(-3) & (2)(-1) + (-1)(2) \\ (-3)(2) + (2)(-3) & (-3)(-1) + (2)(2) \end{pmatrix}$$

Simplify the arithmetic:

$$(A^2)^{-1} = \begin{pmatrix} 4 + 3 & -2 - 2 \\ -6 - 6 & 3 + 4 \end{pmatrix} = \begin{pmatrix} 7 & -4 \\ -12 & 7 \end{pmatrix}$$

---

## Conclusion

Using the properties of matrix inverses, we obtain:
