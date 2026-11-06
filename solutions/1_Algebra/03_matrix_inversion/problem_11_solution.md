# Exercise 11 – Parameter and Invertibility of a Matrix

## Problem

Given the parameter-dependent matrix:

$$A(t) = \begin{pmatrix} 1 & t \\ t & 1 \end{pmatrix}$$

Find all values of $t$ for which the matrix is invertible, determine the formula for $A(t)^{-1}$, and explain what happens to this formula at any excluded values of $t$.

---

## Solution

### Step 1: Understand the invertibility condition for a 2×2 matrix

A square matrix is invertible if and only if its determinant is nonzero:

$$\det(A(t)) \neq 0$$

For a general $2 \times 2$ matrix $M = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$, the determinant is calculated as:

$$\det(M) = ad - bc$$

If $\det(M) \neq 0$, its inverse is given by the formula:

$$M^{-1} = \frac{1}{\det(M)} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix}$$

### Step 2: Calculate the determinant of A(t)

Apply the determinant formula to matrix $A(t)$:

$$\det(A(t)) = (1)(1) - (t)(t) = 1 - t^2$$

### Step 3: Determine the values of t for which A(t) is invertible

Set the determinant unequal to zero:

$$1 - t^2 \neq 0$$

Factor the difference of squares:

$$(1 - t)(1 + t) \neq 0$$

This yields two non-zero conditions:

$$1 - t \neq 0 \implies t \neq 1$$

$$1 + t \neq 0 \implies t \neq -1$$

Thus, matrix $A(t)$ is invertible for all real numbers except $t = 1$ and $t = -1$ (i.e., $t \neq \pm 1$).

### Step 4: Calculate the inverse formula for A(t)

For $t \neq \pm 1$, apply the inverse formula for a $2 \times 2$ matrix:

$$A(t)^{-1} = \frac{1}{\det(A(t))} \begin{pmatrix} 1 & -t \\ -t & 1 \end{pmatrix}$$

Substitute $\det(A(t)) = 1 - t^2$:

$$A(t)^{-1} = \frac{1}{1 - t^2} \begin{pmatrix} 1 & -t \\ -t & 1 \end{pmatrix}, \qquad t \neq \pm 1$$

Or expressed as a single matrix:

$$A(t)^{-1} = \begin{pmatrix} \frac{1}{1 - t^2} & \frac{-t}{1 - t^2} \\ \frac{-t}{1 - t^2} & \frac{1}{1 - t^2} \end{pmatrix}$$

### Step 5: Explain the behavior at the excluded values

At $t = 1$ and $t = -1$:

1. **Determinant evaluates to zero:** $\det(A(1)) = 1 - (1)^2 = 0$ and $\det(A(-1)) = 1 - (-1)^2 = 0$.
2. **Division by zero:** The term $\frac{1}{1 - t^2}$ yields division by zero, making the explicit formula for $A(t)^{-1}$ undefined.
3. **Singularity:** At these values, the rows (and columns) of $A(t)$ become linearly dependent, making the matrix singular (non-invertible). Therefore, no inverse exists for $t = 1$ or $t = -1$.

---

## Conclusion

- Matrix $A(t)$ is invertible for **all $t \neq \pm 1$**.
- For $t \neq \pm 1$, its inverse is:  $$
A(t)^{-1} = \frac{1}{1 - t^2} \begin{pmatrix} 1 &
