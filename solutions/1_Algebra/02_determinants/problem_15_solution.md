# Exercise 15 – Combining Determinant Properties

## Problem

Let $A$ and $B$ be invertible $2 \times 2$ matrices with

$$
\det(A) = -2,
\qquad
\det(B) = 3
$$

Without finding the entries of the matrices, compute:

$$
\det\left(B^{-1}A^TB\right)
$$

State the determinant properties used in order and explain why the factors involving $B$ eventually cancel.

---

## Solution

### Step 1: Apply the multiplicative property of determinants

For any square matrices $X$, $Y$, and $Z$ of the same size, the determinant of a product satisfies:

$$
\det(XYZ) = \det(X) \det(Y) \det(Z)
$$

Applying this property to our expression:

$$
\det\left(B^{-1}A^TB\right) = \det\left(B^{-1}\right) \det\left(A^T\right) \det(B)
$$

---

### Step 2: Evaluate each determinant component

1. **Inverse property:** The determinant of an inverse matrix is the reciprocal of the determinant:

$$
\det\left(B^{-1}\right) = \frac{1}{\det(B)} = \frac{1}{3}
$$

2. **Transpose property:** A matrix and its transpose have equal determinants:

$$
\det\left(A^T\right) = \det(A) = -2
$$

---

### Step 3: Substitute and compute the final value

Substitute the evaluated components into the product:

$$
\det\left(B^{-1}A^TB\right) = \left(\frac{1}{3}\right) (-2) (3)
$$

Simplify the expression:

$$
\det\left(B^{-1}A^TB\right) = -2
$$

---

### Step 4: Explain the cancellation of matrix B factors

The factors involving $B$ cancel out because the determinant of $B^{-1}$ is the multiplicative inverse of the determinant of $B$:

$$
\det\left(B^{-1}\right) \det(B) = \left(\frac{1}{3}\right)(3) = 1
$$

Multiplying by $1$ leaves only the determinant of $A^T$.

---

## Conclusion

- Using determinant properties, the expression breaks down into individual scalar determinants.
- The terms involving matrix $B$ cancel out because $\det\left(B^{-1}\right)\det(B) = 1$.
- The final computed value is:

$$
\det\left(B^{-1}A^TB\right) = -2
$$
