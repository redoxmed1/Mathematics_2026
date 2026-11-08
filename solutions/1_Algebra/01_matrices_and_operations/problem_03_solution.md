# Exercise 3. When Can Matrices Be Multiplied?

## Problem

The matrix sizes are:

A is 2 × 3

B is 3 × 4

C is 4 × 2

D is 2 × 2

For the products:

AB, BA, BC, CB, AC, CA, AD, DA

Determine whether each product is defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

## Solution

### Step 1. Explain the Multiplication Rule

Two matrices can be multiplied if the number of columns of the first matrix equals the number of rows of the second matrix.

The general rule is:

$$
(m\times n)(n\times p)=m\times p
$$

The inner dimensions must be equal, and the outer dimensions determine the size of the resulting matrix.

### Step 2. Check Each Product

**1. Product AB**

$$
A_{2\times3}B_{3\times4}
$$

The inner dimensions are equal:

$$
3=3
$$

Therefore, the product is defined.

The resulting matrix has dimensions:

$$
AB_{2\times4}
$$

**2. Product BA**

$$
B_{3\times4}A_{2\times3}
$$

The inner dimensions are:

$$
4\ne2
$$

Therefore, the product is not defined.

**3. Product BC**

$$
B_{3\times4}C_{4\times2}
$$

The inner dimensions are equal:

$$
4=4
$$

Therefore, the product is defined.

The resulting matrix has dimensions:

$$
BC_{3\times2}
$$

**4. Product CB**

$$
C_{4\times2}B_{3\times4}
$$

The inner dimensions are:

$$
2\ne3
$$

Therefore, the product is not defined.

**5. Product AC**

$$
A_{2\times3}C_{4\times2}
$$

The inner dimensions are:

$$
3\ne4
$$

Therefore, the product is not defined.

**6. Product CA**

$$
C_{4\times2}A_{2\times3}
$$

The inner dimensions are equal:

$$
2=2
$$

Therefore, the product is defined.

The resulting matrix has dimensions:

$$
CA_{4\times3}
$$

**7. Product AD**

$$
A_{2\times3}D_{2\times2}
$$

The inner dimensions are:

$$
3\ne2
$$

Therefore, the product is not defined.

**8. Product DA**

$$
D_{2\times2}A_{2\times3}
$$

The inner dimensions are equal:

$$
2=2
$$

Therefore, the product is defined.

The resulting matrix has dimensions:

$$
DA_{2\times3}
$$

### Step 3. Final Results

The defined products are:

$$
AB:\ 2\times4
$$

$$
BC:\ 3\times2
$$

$$
CA:\ 4\times3
$$

$$
DA:\ 2\times3
$$

The undefined products are:

$$
BA,\quad CB,\quad AC,\quad AD
$$

### Conclusion

Matrix multiplication is possible only when the number of columns of the first matrix equals the number of rows of the second matrix.

When multiplication is possible, the resulting matrix takes its dimensions from the outer numbers.

This exercise demonstrates the importance of checking dimension compatibility before performing matrix multiplication.
