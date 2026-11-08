### Exercise 3. Matrix Multiplication: Dimension Check

**Problem**

Consider four matrices with the following dimensions:

* Matrix A has dimensions 2 × 3.
* Matrix B has dimensions 3 × 4.
* Matrix C has dimensions 4 × 2.
* Matrix D has dimensions 2 × 2.

Determine whether the following matrix products are defined. If a product is defined, give the dimensions of the resulting matrix.

1. AB
2. BA
3. BC
4. CB
5. AC
6. CA
7. AD
8. DA

### Solution

**Rule of Matrix Multiplication**

To multiply two matrices, the number of columns in the first matrix must equal the number of rows in the second matrix.

If the first matrix has dimensions m × n and the second matrix has dimensions n × p, the product is defined and the resulting matrix has dimensions m × p.

**1. Product AB**

A has dimensions 2 × 3, and B has dimensions 3 × 4.

The number of columns of A (3) equals the number of rows of B (3).

Therefore, AB is defined.

Result dimensions: 2 × 4.

**2. Product BA**

B has dimensions 3 × 4, and A has dimensions 2 × 3.

The number of columns of B (4) does not equal the number of rows of A (2).

Therefore, BA is not defined.

**3. Product BC**

B has dimensions 3 × 4, and C has dimensions 4 × 2.

The number of columns of B (4) equals the number of rows of C (4).

Therefore, BC is defined.

Result dimensions: 3 × 2.

**4. Product CB**

C has dimensions 4 × 2, and B has dimensions 3 × 4.

The number of columns of C (2) does not equal the number of rows of B (3).

Therefore, CB is not defined.

**5. Product AC**

A has dimensions 2 × 3, and C has dimensions 4 × 2.

The number of columns of A (3) does not equal the number of rows of C (4).

Therefore, AC is not defined.

**6. Product CA**

C has dimensions 4 × 2, and A has dimensions 2 × 3.

The number of columns of C (2) equals the number of rows of A (2).

Therefore, CA is defined.

Result dimensions: 4 × 3.

**7. Product AD**

A has dimensions 2 × 3, and D has dimensions 2 × 2.

The number of columns of A (3) does not equal the number of rows of D (2).

Therefore, AD is not defined.

**8. Product DA**

D has dimensions 2 × 2, and A has dimensions 2 × 3.

The number of columns of D (2) equals the number of rows of A (2).

Therefore, DA is defined.

Result dimensions: 2 × 3.

### Conclusion

The defined matrix products are:

* AB: 2 × 4
* BC: 3 × 2
* CA: 4 × 3
* DA: 2 × 3

The undefined matrix products are:

* BA
* CB
* AC
* AD

A matrix product is possible only when the inner dimensions of the two matrices are equal.
