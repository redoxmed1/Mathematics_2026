### Exercise 7. Using Properties Instead of Recomputing

**Problem**

Suppose that for a 3 × 3 matrix, the determinant of A is −4. Compute

$$
\det(2A),\qquad
\det(A^T),\qquad
\det(A^2),\qquad
\det(-A).
$$

Justify each answer using the appropriate property.

**Solution**

The given information is

$$
\det A=-4.
$$

**1. Determinant of 2A**

For an n × n matrix, multiplying every row by a scalar c multiplies the determinant by cⁿ. Since A is 3 × 3,

$$
\det(2A)=2^3\det A=8(-4)=-32.
$$

**2. Determinant of the transpose**

A matrix and its transpose have the same determinant:

$$
\det(A^T)=\det A=-4.
$$

**3. Determinant of A²**

The determinant of a product is the product of the determinants:

$$
\det(A^2)=\det(A)\det(A)=(-4)(-4)=16.
$$

**4. Determinant of −A**

Since A is 3 × 3, multiplying A by −1 multiplies its determinant by (−1)³:

$$
\det(-A)=(-1)^3\det A=(-1)(-4)=4.
$$

The four answers are therefore −32, −4, 16, and 4, respectively.

---
