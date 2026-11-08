# Exercise 3. When Can Matrices Be Multiplied?

## Problem

Given four matrices with the following dimensions:

$$
A=
\begin{pmatrix}
a_{11} & a_{12} & a_{13}\\
a_{21} & a_{22} & a_{23}
\end{pmatrix}
$$

$$
B=
\begin{pmatrix}
b_{11} & b_{12} & b_{13} & b_{14}\\
b_{21} & b_{22} & b_{23} & b_{24}\\
b_{31} & b_{32} & b_{33} & b_{34}
\end{pmatrix}
$$

$$
C=
\begin{pmatrix}
c_{11} & c_{12}\\
c_{21} & c_{22}\\
c_{31} & c_{32}\\
c_{41} & c_{42}
\end{pmatrix}
$$

$$
D=
\begin{pmatrix}
d_{11} & d_{12}\\
d_{21} & d_{22}
\end{pmatrix}
$$

For the following products:

AB, BA, BC, CB, AC, CA, AD, and DA,

determine whether each product is defined. If it is defined, state the dimensions of the resulting matrix.

Justify each decision using the dimension compatibility condition.

## Solution

### Step 1. Explain the Multiplication Rule

Two matrices can be multiplied when the number of columns of the first matrix equals the number of rows of the second matrix.

The general rule is:

$$
(m\times n)(n\times p)=m\times p
$$

The inner dimensions must be equal, and the outer dimensions determine the size of the result.

### Step 2. Check All Eight Products

**1. Product AB**

$$
A_{2\times3}B_{3\times4}
$$

The inner dimensions are equal:

$$
3=3
$$

Therefore, AB is defined.

The resulting matrix has dimensions:

$$
AB_{2\times4}
$$

**2. Product BA**

$$
B_{3\times4}A_{2\times3}
$$

The inner dimensions are not equal:

$$
4\ne2
$$

Therefore, BA is not defined.

**3. Product BC**

$$
B_{3\times4}C_{4\times2}
$$

The inner dimensions are equal:

$$
4=4
$$

Therefore, BC is defined.

The resulting matrix has dimensions:

$$
BC_{3\times2}
$$

**4. Product CB**

$$
C_{4\times2}B_{3\times4}
$$

The inner dimensions are not equal:

$$
2\ne3
$$

Therefore, CB is not defined.

**5. Product AC**

$$
A_{2\times3}C_{4\times2}
$$

The inner dimensions are not equal:

$$
3\ne4
$$

Therefore, AC is not defined.

**6. Product CA**

$$
C_{4\times2}A_{2\times3}
$$

The inner dimensions are equal:

$$
2=2
$$

Therefore, CA is defined.

The resulting matrix has dimensions:

$$
CA_{4\times3}
$$

**7. Product AD**

$$
A_{2\times3}D_{2\times2}
$$

The inner dimensions are not equal:

$$
3\ne2
$$

Therefore, AD is not defined.

**8. Product DA**

$$
D_{2\times2}A_{2
$$
