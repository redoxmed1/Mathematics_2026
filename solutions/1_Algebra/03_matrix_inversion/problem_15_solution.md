# Exercise 15 – Two Methods for Solving the Same System

## Problem

Given

$$
A = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix},
\qquad
b = \begin{pmatrix} 7 \\ 8 \end{pmatrix}
$$

solve $Ax = b$ in two ways:

1. Using $x = A^{-1}b$.
2. Using Gaussian elimination.

Compare both solutions, count the essential arithmetic operations, and identify which method is simpler in this example.

---

## Solution

### Method 1: Using the inverse matrix

#### Step 1: Calculate the determinant of A
Apply the $2 \times 2$ determinant formula:

$$
\det(A) = (2)(3) - (1)(1) = 6 - 1 = 5
$$

Since the determinant is nonzero ($\det(A) \neq 0$), matrix $A$ is invertible.

#### Step 2: Calculate the inverse of A
Apply the $2 \times 2$ inverse formula:

$$
A^{-1} = \frac{1}{5} \begin{pmatrix} 3 & -1 \\ -1 & 2 \end{pmatrix}
$$

$$
A^{-1} = \begin{pmatrix} \frac{3}{5} & -\frac{1}{5} \\ -\frac{1}{5} & \frac{2}{5} \end{pmatrix}
$$

#### Step 3: Compute x = A⁻¹b
Multiply $A^{-1}$ by vector $b$:

$$
x = \begin{pmatrix} \frac{3}{5} & -\frac{1}{5} \\ -\frac{1}{5} & \frac{2}{5} \end{pmatrix} \begin{pmatrix} 7 \\ 8 \end{pmatrix}
$$

Calculate each entry:

$$
x = \begin{pmatrix} \left(\frac{3}{5}\right)(7) + \left(-\frac{1}{5}\right)(8) \\ \left(-\frac{1}{5}\right)(7) + \left(\frac{2}{5}\right)(8) \end{pmatrix}
$$

$$
x = \begin{pmatrix} \frac{21 - 8}{5} \\ \frac{-7 + 16}{5} \end{pmatrix} = \begin{pmatrix} \frac{13}{5} \\ \frac{9}{5} \end{pmatrix}
$$

#### Operation count for Method 1
1. **Determinant:** 2 multiplications and 1 subtraction = 3 operations.
2. **Inverse entries:** 4 scalar divisions by 5 = 4 operations.
3. **Matrix-vector product:** 4 multiplications and 2 additions = 6 operations.

**Total operations for Method 1:** $3 + 4 + 6 = 13$ operations.

---

### Method 2: Using Gaussian elimination

#### Step 1: Set up the augmented matrix
Write the augmented matrix $\left(A \mid b\right)$:

$$
\left(
\begin{array}{cc|c}
2 & 1 & 7 \\
1 & 3 & 8
\end{array}
\right)
$$

#### Step 2: Swap the rows for a clean pivot
Apply row swap $R_1 \leftrightarrow R_2$:

$$
\left(
\begin{array}{cc|c}
1 & 3 & 8 \\
2 & 1 & 7
\end{array}
\right)
$$

#### Step 3: Eliminate the first entry in row 2
Apply operation $R_2 \to R_2 - 2R_1$:

$$
\left(
\begin{array}{cc|c}
1 & 3 & 8 \\
0 & -5 & -9
\end{array}
\right)
$$

#### Step 4: Normalize the second row pivot
Apply operation $R_2 \to -\frac{1}{5}R_2$:

$$
\left(
\begin{array}{cc|c}
1 & 3 & 8 \\
0 & 1 & \frac{9}{5}
\end{array}
\right)
$$

#### Step 5: Eliminate the upper entry in column 2
Apply operation $R_1 \to R_1 - 3R_2$:

$$
\left(
\begin{array}{cc|c}
1 & 0 & \frac{13}{5} \\
0 & 1 & \frac{9}{5}
\end{array}
\right)
$$

Thus, the solution vector is:

$$
x = \begin{pmatrix} \frac{13}{5} \\ \frac{9}{5} \end{pmatrix}
$$

#### Operation count for Method 2
1. **Row interchange:** 0 arithmetic operations.
2. **First elimination step:** 3 multiplications and 3 subtractions = 6 operations.
3. **Row normalization:** 3 scalar multiplications = 3 operations.
4. **Second elimination step:** 3 multiplications and 3 subtractions = 6 operations.

**Total operations for Method 2:** $6 + 3 + 6 = 15$ operations.

---

## Comparison and Verification

### Comparison of Methods

| Method | Arithmetic Operations |
| :--- | :---: |
| **Inverse Matrix Method ($x = A^{-1}b$)** | 13 |
| **Gaussian Elimination** | 15 |

- Both methods yield the exact same solution: $x = \begin{pmatrix} \frac{13}{5} \\ \frac{9}{5} \end{pmatrix}$.
- In this specific $2 \times 2$ example, the inverse method requires 2 fewer operations ($15 - 13 = 2$).
- However, Gaussian elimination is generally far more efficient and numerically stable for larger systems ($n > 3$) because it avoids computing the explicit inverse matrix.

### Final Verification

Substitute the solution back into $Ax$:

$$
Ax = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix} \begin{pmatrix} \frac{13}{5} \\ \frac{9}{5} \end{pmatrix} = \begin{pmatrix} \frac{26}{5} + \frac{9}{5} \\ \frac{13}{5} + \frac{27}{5} \end{pmatrix} = \begin{pmatrix} \frac{35}{5} \\ \frac{40}{5} \end{pmatrix} = \begin{pmatrix} 7 \\ 8 \end{pmatrix} = b
$$

The calculation matches vector $b$, confirming that the solution is correct.

---

## Conclusion

- Both methods solve the linear system successfully.
- According to the arithmetic operation count, the inverse method is slightly shorter for this particular $2 \times 2$ matrix.
- For practical applications involving larger matrices, Gaussian elimination remains the preferred choice.
