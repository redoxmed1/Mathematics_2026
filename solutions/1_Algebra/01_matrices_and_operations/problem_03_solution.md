# Exercise 3. When Can Matrices Be Multiplied?

## Problem

The matrix sizes are:

$$
A_{2\times3},\qquad
B_{3\times4},\qquad
C_{4\times2},\qquad
D_{2\times2}
$$

For the following products:

$$
AB,\quad BA,\quad BC,\quad CB,
$$

$$
AC,\quad CA,\quad AD,\quad DA
$$

determine whether each product is defined.

If it is defined, state the size of the resulting matrix.

Justify each decision using the dimension compatibility condition.

## Solution

### Step 1. Explain the Multiplication Rule

Two matrices can be multiplied when the number of columns of the first matrix equals the number of rows of the second matrix.

If the first matrix has dimensions m × n and the second matrix has dimensions n × p, the resulting matrix has dimensions m × p.

Therefore, the rule is:

$$
(m\times n)(n\times p)=m\times p
$$

### Step 2. Calculate and Check All Eight Products

**1. Product AB**

The dimensions are:

$$
A_{2\times3}B_{3\times4}
$$

The inner dimensions are equal:

$$
3=3
$$

Therefore, the product is defined.

The resulting dimensions are:

$$
AB \text{ is } 2\times4
$$

**2. Product BA**

$$
B_{3\times4}A_{2\times3}
$$

The inner dimensions are:

$$
4\ne2
$$

Therefore, BA is not defined.

**3. Product BC**

$$
B_{3\times4}C_{4\times2}
$$

The inner dimensions are:

$$
4=4
$$

Therefore, the product is defined.

The resulting dimensions are:

$$
BC \text{ is } 3\times2
$$

**4. Product CB**

$$
C_{4\times2}B_{3\times4}
$$

The inner dimensions are:

$$
2\ne3
$$

Therefore, CB is not defined.

**5. Product AC**

$$
A_{2\times3}C_{4\times2}
$$

The inner dimensions are:

$$
3\ne4
$$

Therefore, AC is not defined.

**6. Product CA**

$$
C_{4\times2}A_{2\times3}
$$

The inner dimensions are:

$$
2=2
$$

Therefore, the product is defined.

The resulting dimensions are:

$$
CA \text{ is } 4\times3
$$

**7. Product AD**

$$
A_{2\times3}D_{2\times2}
$$

The inner dimensions are:

$$
3\ne2
$$

Therefore, AD is not defined.

**8. Product DA**

$$
D_{2\times2}A_{2\times3}
$$

The inner dimensions are:

$$
2=2
$$

Therefore, the product is defined.

The resulting dimensions are:

$$
DA \text{ is } 2\times3
$$

### Step 3. Final Results

The results are:

$$
AB \text{ is } 2\times4
$$

$$
BA \text{ is not defined}
$$

$$
BC \text{ is } 3\times2
$$

$$
CB \text{ is not defined}
$$

$$
AC \text{ is not defined}
$$

$$
CA \text{ is } 4\times3
$$

$$
AD \text{ is not defined}
$$

$$
DA \text{ is } 2\times3
$$

### Conclusion

Matrix multiplication is possible only when the number of columns of the first matrix equals the number of rows of the second matrix.

For every defined product, the resulting matrix takes its dimensions from the outside numbers.

---
