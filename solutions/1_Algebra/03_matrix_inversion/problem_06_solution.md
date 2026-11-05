
# Exercise 6: Solving a System Using the Inverse

## Problem

Solve the equation Ax = b using the inverse matrix method.

Given:

$$
A = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix}
$$

$$
b = \begin{pmatrix} 5 \\ 7 \end{pmatrix}
$$

Use the formula:

$$
x = A^{-1}b
$$

Then substitute the result into the original equation to check the answer.

---

## Solution

### Step 1: Calculate the determinant

$$
\det(A) = 2(3) - 1(1)
$$

$$
\det(A) = 6 - 1 = 5
$$

Since the determinant is not zero, the inverse matrix exists.

### Step 2: Calculate the inverse matrix

The inverse formula for a 2x2 matrix is:

$$
A^{-1} = \frac{1}{ad-bc}
\begin{pmatrix} d & -b \\ -c & a \end{pmatrix}
$$

Substitute the values:

$$
A^{-1} = \frac{1}{5}
\begin{pmatrix} 3 & -1 \\ -1 & 2 \end{pmatrix}
$$

### Step 3: Calculate x = A^-1 b

$$
x = \frac{1}{5}
\begin{pmatrix} 3 & -1 \\ -1 & 2 \end{pmatrix}
\begin{pmatrix} 5 \\ 7 \end{pmatrix}
$$

Multiply the matrices:

$$
x = \frac{1}{5}
\begin{pmatrix} 3(5)-1(7) \\ -1(5)+2(7) \end{pmatrix}
$$

$$
x = \frac{1}{5}
\begin{pmatrix} 8 \\ 9 \end{pmatrix}
$$

Therefore:

$$
x = \begin{pmatrix} 8/5 \\ 9/5 \end{pmatrix}
$$

---

## Verification

Substitute the result into the original equation Ax = b:

$$
Ax =
\begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix}
\begin{pmatrix} 8/5 \\ 9/5 \end{pmatrix}
$$

Calculate each entry:

$$
Ax =
\begin{pmatrix}
2(8/5)+9/5 \\
8/5+3(9/5)
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
25/5 \\
35/5
\end{pmatrix}
$$

$$
Ax = \begin{pmatrix} 5 \\ 7 \end{pmatrix} = b
$$

The result is equal to the original vector b, so the solution is correct.

---

## Final Answer

$$
x = \begin{pmatrix} 8/5 \\ 9/5 \end{pmatrix}
$$

**Conclusion:** The system has a unique solution, and substitution confirms that the answer is correct.
