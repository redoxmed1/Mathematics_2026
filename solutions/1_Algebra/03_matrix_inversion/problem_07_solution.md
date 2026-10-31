
### Exercise 7. Inverse of a Product

**Problem**

For the matrices

A = [[1, 1], [0, 1]]

B = [[2, 0], [0, 3]]

Compute (AB)^-1 and B^-1 A^-1. Check that the results are the same and explain why the inverse of a product reverses the order of the factors.

**Solution**

**1. Calculate AB**

Multiply the rows of A by the columns of B:

AB = [[1(2)+1(0), 1(0)+1(3)],
      [0(2)+1(0), 0(0)+1(3)]]

AB = [[2, 3],
      [0, 3]]

**2. Calculate (AB)^-1**

First calculate the determinant:

det(AB) = 2(3) - 3(0) = 6

Since the determinant is nonzero, the inverse exists.

Using the 2 x 2 inverse formula:

(AB)^-1 = (1/6) [[3, -3],
                  [0,  2]]

Therefore:

(AB)^-1 = [[1/2, -1/2],
           [0,    1/3]]

**3. Calculate A^-1 and B^-1 separately**

For A:

det(A) = 1(1) - 1(0) = 1

A^-1 = [[1, -1],
        [0,  1]]

For B:

det(B) = 2(3) - 0(0) = 6

B^-1 = [[1/2, 0],
        [0, 1/3]]

**4. Calculate B^-1 A^-1**

Multiply the inverses in the reversed order:

B^-1 A^-1 = [[1/2, 0],
              [0, 1/3]]
             [[1, -1],
              [0,  1]]

B^-1 A^-1 = [[1/2(1)+0(0), 1/2(-1)+0(1)],
              [0(1)+1/3(0), 0(-1)+1/3(1)]]

B^-1 A^-1 = [[1/2, -1/2],
              [0,    1/3]]

Both methods give the same result:

(AB)^-1 = B^-1 A^-1

**5. Explanation of the reversed order**

When we calculate ABx, the matrix B acts on the vector x first, and then A acts on the result.

To undo these operations, we must reverse their order.

First, A is undone using A^-1. Then, B is undone using B^-1.

Therefore:

A^-1(ABx) = Bx

B^-1(A^-1(ABx)) = x

This gives the inverse product:

(AB)^-1 = B^-1 A^-1

**Conclusion**

The inverse of a product reverses the order of the original matrices because the last transformation applied must be the first one undone. The calculations confirm that both methods produce the same inverse matrix.

