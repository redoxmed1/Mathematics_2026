# Exercise 7. Inverse of a Product

## Problem

Given the matrices:

A =

| 1 | 1 |
| - | - |
| 0 | 1 |

B =

| 2 | 0 |
| - | - |
| 0 | 3 |

Compute (AB)⁻¹ and B⁻¹A⁻¹.

Check that the results are the same and explain the meaning of the reversed order.

## Solution

### Step 1. Calculate the product AB

First, we multiply matrix A by matrix B. We multiply each row of A by each column of B.

AB =

| 1×2 + 1×0 | 1×0 + 1×3 |
| --------- | --------- |
| 0×2 + 1×0 | 0×0 + 1×3 |

Therefore:

AB =

| 2 | 3 |
| - | - |
| 0 | 3 |

### Step 2. Calculate the inverse of AB

For a 2×2 matrix, the inverse is obtained by dividing the matrix with exchanged diagonal elements and opposite off-diagonal elements by its determinant.

The determinant of AB is:

det(AB) = (2×3) - (3×0)

det(AB) = 6

Since the determinant is not zero, the inverse exists.

Therefore:

(AB)⁻¹ =

| 3/6 | -3/6 |
| --- | ---- |
| 0/6 | 2/6  |

Simplifying:

(AB)⁻¹ =

| 1/2 | -1/2 |
| --- | ---- |
| 0   | 1/3  |

### Step 3. Calculate A⁻¹ and B⁻¹

First, we calculate the inverse of A.

det(A) = (1×1) - (1×0) = 1

Therefore:

A⁻¹ =

| 1 | -1 |
| - | -- |
| 0 | 1  |

Next, we calculate the inverse of B.

det(B) = (2×3) - (0×0) = 6

Therefore:

B⁻¹ =

| 1/2 | 0   |
| --- | --- |
| 0   | 1/3 |

### Step 4. Calculate B⁻¹A⁻¹

Now, we multiply B⁻¹ by A⁻¹.

B⁻¹A⁻¹ =

| (1/2×1) + (0×0) | (1/2×-1) + (0×1) |
| --------------- | ---------------- |
| (0×1) + (1/3×0) | (0×-1) + (1/3×1) |

Therefore:

B⁻¹A⁻¹ =

| 1/2 | -1/2 |
| --- | ---- |
| 0   | 1/3  |

### Step 5. Compare the results

From Step 2:

(AB)⁻¹ =

| 1/2 | -1/2 |
| --- | ---- |
| 0   | 1/3  |

From Step 4:

B⁻¹A⁻¹ =

| 1/2 | -1/2 |
| --- | ---- |
| 0   | 1/3  |

Both matrices are identical.

Therefore:

(AB)⁻¹ = B⁻¹A⁻¹

### Step 6. Explain the reversed order

The inverse of a product reverses the order of multiplication.

When we calculate AB, matrix B acts first and matrix A acts second.

To undo these operations, we must first undo A using A⁻¹ and then undo B using B⁻¹.

This is why the inverse of AB is B⁻¹A⁻¹ rather than A⁻¹B⁻¹.

**Conclusion:**

The calculations confirm that the inverse of a product is equal to the product of the inverses in reversed order.

(AB)⁻¹ = B⁻¹A⁻¹
