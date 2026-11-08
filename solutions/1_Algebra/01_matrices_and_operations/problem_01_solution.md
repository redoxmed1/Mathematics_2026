# Exercise 1. Matrix Size and Entries

## Problem

Given

$$
A=
\begin{pmatrix}
2 & -1 & 3\\
0 & 4 & 5
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
1 & 0\\
-2 & 3\\
4 & 1
\end{pmatrix}
$$

1. State the sizes of matrices A and B.
2. Identify the entries a₁₂, a₂₃, b₂₁, and b₃₂.
3. Write the second row of A and the first column of B as vectors.

## Solution

### Step 1. Determine the Matrix Sizes

The size of a matrix is determined by counting its rows and columns.

Matrix A has 2 rows and 3 columns.

Therefore:

$$
A \text{ is } 2\times 3
$$

Matrix B has 3 rows and 2 columns.

Therefore:

$$
B \text{ is } 3\times 2
$$

### Step 2. Identify the Matrix Entries

In matrix notation, the first index represents the row and the second index represents the column.

For matrix A:

* a₁₂ is in row 1, column 2, so a₁₂ = -1.
* a₂₃ is in row 2, column 3, so a₂₃ = 5.

For matrix B:

* b₂₁ is in row 2, column 1, so b₂₁ = -2.
* b₃₂ is in row 3, column 2, so b₃₂ = 1.

### Step 3. Write the Required Vectors

The second row of A is:

$$
\begin{pmatrix}
0 & 4 & 5
\end{pmatrix}
$$

The first column of B is:

$$
\begin{pmatrix}
1\\
-2\\
4
\end{pmatrix}
$$

### Conclusion

The dimensions are A = 2 × 3 and B = 3 × 2.

The required entries are:

$$
a_{12}=-1,\quad
a_{23}=5,\quad
b_{21}=-2,\quad
b_{32}=1
$$

The second row of A and the first column of B have been correctly identified.

---

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

# Exercise 4. Matrix Multiplication and Noncommutativity

## Problem

Given

$$
A=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

1. Compute AB and BA.
2. Determine whether AB = BA.
3. Explain what noncommutativity of matrix multiplication means.

## Solution

### Step 1. Calculate AB

To multiply two matrices, each entry is obtained by multiplying a row of the first matrix by a column of the second matrix.

$$
AB=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

Calculate each entry:

$$
AB=
\begin{pmatrix}
1(2)+2(3) & 1(0)+2(1)\\
0(2)+1(3) & 0(0)+1(1)
\end{pmatrix}
$$

Simplifying:

$$
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
$$

### Step 2. Calculate BA

Now reverse the order of multiplication.

$$
BA=
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

Calculate each entry:

$$
BA=
\begin{pmatrix}
2(1)+0(0) & 2(2)+0(1)\\
3(1)+1(0) & 3(2)+1(1)
\end{pmatrix}
$$

Simplifying:

$$
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

### Step 3. Compare the Results

We obtained:

$$
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
$$

And:

$$
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

The matrices are different because their corresponding entries are not equal.

Therefore:

$$
\boxed{AB\ne BA}
$$

### Step 4. Explain Noncommutativity

Noncommutativity means that changing the order of matrix multiplication can produce a different result.

In ordinary number multiplication, changing the order does not change the answer.

For example:

$$
2\times3=3\times2=6
$$

However, for matrices:

$$
AB\ne BA
$$

as demonstrated by our calculations.

### Conclusion

This example proves that matrix multiplication is generally not commutative.

The order of the matrices matters, and multiplying A by B can produce a different result from multiplying B by A.

---

# Exercise 10. Columns of a Matrix Product

## Problem

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
1 & 2\\
-1 & 0\\
3 & 1
\end{pmatrix}
$$

Denote the columns of B by b₁ and b₂.

1. Compute Ab₁ and Ab₂.
2. Compute the matrix AB.
3. Compare the results and explain why the columns of AB are exactly the vectors Ab₁ and Ab₂.

## Solution

### Step 1. Identify the Columns of B

The first column of B is:

$$
b_1=
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}
$$

The second column of B is:

$$
b_2=
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
$$

### Step 2. Calculate Ab₁

Multiply matrix A by the first column of B.

$$
Ab_1=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}
$$

Multiply each row by the column vector:

$$
Ab_1=
\begin{pmatrix}
1(1)+2(-1)+0(3)\\
0(1)+1(-1)+1(3)
\end{pmatrix}
$$

Simplifying:

$$
Ab_1=
\begin{pmatrix}
-1\\
2
\end{pmatrix}
$$

### Step 3. Calculate Ab₂

Multiply matrix A by the second column of B.

$$
Ab_2=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
$$

Multiply each row by the column vector:

$$
Ab_2=
\begin{pmatrix}
1(2)+2(0)+0(1)\\
0(2)+1(0)+1(1)
\end{pmatrix}
$$

Simplifying:

$$
Ab_2=
\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

### Step 4. Calculate the Matrix AB

Now multiply the complete matrices A and B.

$$
AB=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2\\
-1 & 0\\
3 & 1
\end{pmatrix}
$$

Calculate each entry:

$$
AB=
\begin{pmatrix}
1(1)+2(-1)+0(3) & 1(2)+2(0)+0(1)\\
0(1)+1(-1)+1(3) & 0(2)+1(0)+1(1)
\end{pmatrix}
$$

Simplifying:

$$
AB=
\begin{pmatrix}
-1 & 2\\
2 & 1
\end{pmatrix}
$$

### Step 5. Compare the Results

From our calculations:

$$
Ab_1=
\begin{pmatrix}
-1\\
2
\end{pmatrix}
$$

And:

$$
Ab_2=
\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

The complete product is:

$$
AB=
\begin{pmatrix}
-1 & 2\\
2 & 1
\end{pmatrix}
$$

We can see that the first column of AB is exactly Ab₁, and the second column is exactly Ab₂.

Therefore:

$$
AB=
\begin{pmatrix}
| & |\\
Ab_1 & Ab_2\\
| & |
\end{pmatrix}
$$

### Conclusion

Matrix multiplication applies matrix A separately to each column of matrix B.

That is why the columns of AB are exactly the vectors Ab₁ and Ab₂.

The calculations confirm this property:

$$
\boxed{AB=\begin{pmatrix}Ab_1 & Ab_2\end{pmatrix}}
$$
