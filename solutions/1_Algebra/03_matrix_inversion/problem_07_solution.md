
### Exercise 7. Inverse of a Product

**Problem**

Given the matrices:

A = ⎛ 1  1 ⎞
    ⎝ 0  1 ⎠

B = ⎛ 2  0 ⎞
    ⎝ 0  3 ⎠

Calculate (AB)⁻¹ and B⁻¹A⁻¹. Check that both results are equal and explain why the inverse of a product reverses the order of the factors.

**Solution**

**1. Calculate AB**

Multiply the rows of A by the columns of B:

AB = ⎛ 1(2)+1(0)   1(0)+1(3) ⎞
     ⎝ 0(2)+1(0)   0(0)+1(3) ⎠

AB = ⎛ 2  3 ⎞
     ⎝ 0  3 ⎠

**2. Calculate (AB)⁻¹**

First calculate the determinant:

det(AB) = 2(3) - 3(0) = 6

Since the determinant is not zero, the inverse exists.

Using the inverse formula for a 2 × 2 matrix:

             1    ⎛  d   -b ⎞
A⁻¹ = ─────────── ⎜         ⎟
       ad - bc    ⎝ -c    a ⎠

Therefore:

          1    ⎛  3  -3 ⎞
(AB)⁻¹ = ───   ⎜       ⎟
          6    ⎝  0   2 ⎠

(AB)⁻¹ = ⎛  1/2  -1/2 ⎞
          ⎝   0    1/3 ⎠

**3. Calculate A⁻¹ and B⁻¹ separately**

For matrix A:

det(A) = 1(1) - 1(0) = 1

Therefore:

A⁻¹ = ⎛ 1  -1 ⎞
      ⎝ 0   1 ⎠

For matrix B:

det(B) = 2(3) - 0(0) = 6

Therefore:

B⁻¹ = ⎛ 1/2   0   ⎞
      ⎝  0   1/3  ⎠

**4. Calculate B⁻¹A⁻¹**

Multiply the inverses in the reversed order:

B⁻¹A⁻¹ = ⎛ 1/2   0  ⎞ ⎛ 1  -1 ⎞
          ⎝  0   1/3 ⎠ ⎝ 0   1 ⎠

Multiply rows by columns:

B⁻¹A⁻¹ = ⎛ (1/2)(1)+(0)(0)    (1/2)(-1)+(0)(1) ⎞
          ⎝ (0)(1)+(1/3)(0)   (0)(-1)+(1/3)(1) ⎠

Simplifying:

B⁻¹A⁻¹ = ⎛ 1/2  -1/2 ⎞
          ⎝  0    1/3 ⎠

Both methods give the same result:

(AB)⁻¹ = B⁻¹A⁻¹

**5. Explanation of the reversed order**

When we calculate ABx, matrix B acts on the vector x first, and then matrix A acts on the result.

To undo these operations, we must reverse their order.

First, we undo A using A⁻¹. Then, we undo B using B⁻¹.

Therefore:

A⁻¹(ABx) = Bx

B⁻¹(A⁻¹(ABx)) = x

This proves that:

(AB)⁻¹ = B⁻¹A⁻¹

**Conclusion**

The inverse of a product reverses the order of the original matrices because the last transformation applied must be the first one undone. The calculations confirm that both methods produce the same inverse matrix.


