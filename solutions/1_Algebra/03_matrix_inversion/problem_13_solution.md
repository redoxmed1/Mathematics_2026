### Exercise 13. Undoing a Composite Transformation

**Problem**

The matrices

S = [2  0]
    [0  1]

H = [1  1]
    [0  1]

describe nonuniform scaling and shear.

For T = HS, find T⁻¹ in two ways:

1. First calculate T, then calculate its inverse.
2. Use the property (HS)⁻¹ = S⁻¹H⁻¹.

Compare the results. Additionally, calculate H⁻¹S⁻¹ and verify that using the incorrect order gives a different matrix.

Explain the rule: "When undoing a composition of operations, we undo them from the end."

**Solution**

**Method 1. Calculate T first, then invert it**

Since T = HS, we multiply H by S:

T = [1  1] × [2  0]
    [0  1]   [0  1]

Calculate each entry:

T = [1(2)+1(0)   1(0)+1(1)]
    [0(2)+1(0)   0(0)+1(1)]

Therefore:

T = [2  1]
    [0  1]

**Calculate the determinant**

det(T) = (2 × 1) - (1 × 0)

det(T) = 2

Since the determinant is not zero, the inverse exists.

**Calculate the inverse of T**

For a 2 × 2 matrix:

T = [a  b]
    [c  d]

The inverse is:

T⁻¹ = 1/(ad - bc) × [ d  -b]
                      [-c   a]

Substitute the values:

T⁻¹ = 1/2 × [1  -1]
             [0   2]

Therefore:

T⁻¹ = [1/2  -1/2]
      [ 0     1  ]


**Method 2. Reverse the order of the inverses**

First, calculate the inverse of S:

S = [2  0]
    [0  1]

S⁻¹ = [1/2  0]
      [ 0   1]

Now calculate the inverse of H:

H = [1  1]
    [0  1]

H⁻¹ = [1  -1]
      [0   1]

Using the inverse of a product property:

(HS)⁻¹ = S⁻¹H⁻¹

Calculate:

S⁻¹H⁻¹ = [1/2  0] × [1  -1]
          [ 0   1]   [0   1]

Multiply the matrices:

S⁻¹H⁻¹ = [1/2(1)+0(0)   1/2(-1)+0(1)]
          [0(1)+1(0)     0(-1)+1(1)]

Therefore:

S⁻¹H⁻¹ = [1/2  -1/2]
          [ 0     1  ]

Both methods give the same result:

T⁻¹ = [1/2  -1/2]
      [ 0     1  ]


**Check the incorrect order**

Now calculate H⁻¹S⁻¹:

H⁻¹S⁻¹ = [1  -1] × [1/2  0]
          [0   1]   [ 0   1]

Multiply the matrices:

H⁻¹S⁻¹ = [1(1/2)+(-1)(0)   1(0)+(-1)(1)]
          [0(1/2)+1(0)      0(0)+1(1)]

Therefore:

H⁻¹S⁻¹ = [1/2  -1]
          [ 0    1]

This result is different from the correct inverse because the upper-right entry is -1 instead of -1/2.

Therefore, the order of multiplication is important.


**Geometric Explanation**

The transformation T = HS applies S first and then H.

To undo the complete transformation, we must undo H first and then undo S.

This is why the correct inverse is:

T⁻¹ = S⁻¹H⁻¹

It is not equal to H⁻¹S⁻¹.


**Conclusion**

Both methods give the same correct inverse:

T⁻¹ = [1/2  -1/2]
      [ 0     1  ]

The calculation of H⁻¹S⁻¹ gives a different matrix:

H⁻¹S⁻¹ = [1/2  -1]
          [ 0    1]

This confirms that the order of matrix multiplication matters.

The general rule is:

(AB)⁻¹ = B⁻¹A⁻¹

When finding the inverse of a product, we must reverse the order of the matrices.

Therefore, the exercise confirms that to undo a composition of transformations, we must undo the operations in reverse order.
