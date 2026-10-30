# Determinants — Complete Solutions

## Basic Exercises

### Exercise 1. Determinant of a 2×2 Matrix

**Problem**

Compute

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4
\end{pmatrix},
\qquad
\det
\begin{pmatrix}
1 & 7 \\
2 & 14
\end{pmatrix}.
$$

Which matrix is invertible? Justify the answer.

**Solution**

For a 2 × 2 matrix, the determinant is the product of the main diagonal entries minus the product of the other diagonal entries.

For the first matrix,

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4
\end{pmatrix}
=3(4)-(-2)(5)
=12+10
=22.
$$

For the second matrix,

$$
\det
\begin{pmatrix}
1 & 7 \\
2 & 14
\end{pmatrix}
=1(14)-7(2)
=14-14
=0.
$$

A square matrix is invertible exactly when its determinant is nonzero. Therefore, the first matrix is invertible because its determinant is 22. The second matrix is not invertible because its determinant is zero.

---

### Exercise 2. Determinant of a 3×3 Matrix

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{pmatrix}
$$

compute the determinant using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

**Solution**

For Sarrus' rule, add the products of the three diagonals moving down to the right, and subtract the products of the three diagonals moving up to the right.

The positive diagonal products are

$$
1(3)(5)=15,
\qquad
2(4)(2)=16,
\qquad
(-1)(0)(1)=0.
$$

Their sum is

$$
15+16+0=31.
$$

The negative diagonal products are

$$
(-1)(3)(2)=-6,
\qquad
2(0)(5)=0,
\qquad
1(4)(1)=4.
$$

Their sum is

$$
-6+0+4=-2.
$$

Therefore,

$$
\det A=31-(-2)=33.
$$

**Check using a row operation**

Replace the third row by the third row minus twice the first row:

$$
R_3\leftarrow R_3-2R_1.
$$

Adding a multiple of one row to another row does not change the determinant. The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}.
$$

Expanding along the first column gives

$$
\det A
=1
\begin{vmatrix}
3 & 4 \\
-3 & 7
\end{vmatrix}
=1(3(7)-4(-3))
=21+12
=33.
$$

The check agrees with Sarrus' rule.

---

### Exercise 3. Swapping Two Rows

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
$$

compute the determinant. Then form a matrix B by swapping the first and second rows of A. First predict the determinant of B using a determinant property, and then verify the prediction by calculation.

**Solution**

First calculate the determinant of A by expanding along the first row:

$$
\begin{aligned}
\det A
&=1
\begin{vmatrix}
3 & 1 \\
1 & 1
\end{vmatrix}
-2
\begin{vmatrix}
0 & 1 \\
2 & 1
\end{vmatrix}
+0
\\
&=1(3(1)-1(1))-2(0(1)-1(2))
\\
&=2-2(-2)
\\
&=6.
\end{aligned}
$$

Swapping two rows changes the sign of a determinant. Therefore, before calculating B, the predicted value is

$$
\det B=-\det A=-6.
$$

After swapping the first and second rows,

$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}.
$$

Calculate its determinant by expanding along the first row:

$$
\begin{aligned}
\det B
&=0
-3
\begin{vmatrix}
1 & 0 \\
2 & 1
\end{vmatrix}
+1
\begin{vmatrix}
1 & 2 \\
2 & 1
\end{vmatrix}
\\
&=-3(1(1)-0(2))+(1(1)-2(2))
\\
&=-3-3
\\
&=-6.
\end{aligned}
$$

The direct calculation confirms the prediction: swapping two rows changes the determinant from 6 to −6.

---

### Exercise 4. Triangular Matrix

**Problem**

Without expanding the determinant, compute

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}.
$$

State the rule for an arbitrary triangular matrix and explain it using this example.

**Solution**

A triangular matrix has zeros either above or below its main diagonal. Its determinant is the product of the entries on the main diagonal.

For the given upper triangular matrix, the diagonal entries are 2, −3, and 7. Therefore,

$$
\det A=2(-3)(7)=-42.
$$

The rule is that the determinant of any square triangular matrix equals the product of its diagonal entries. Here, the result is −42, so the matrix is invertible because this determinant is nonzero.

---

### Exercise 5. Row Operations

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

find the determinant by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

**Solution**

Use row replacements to create zeros below the first entry. A row replacement of the form “one row plus a multiple of another row” does not change the determinant.

Start with

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}.
$$

**Step 1.** Apply

$$
R_2\leftarrow R_2-2R_1.
$$

This operation does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}.
$$

**Step 2.** Apply

$$
R_3\leftarrow R_3+R_1.
$$

This operation also does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}.
$$

The first column now has zeros below the first entry. Expanding along that column gives

$$
\begin{aligned}
\det A
&=
\begin{vmatrix}
-3 & -6 \\
6 & 5
\end{vmatrix}
\\
&=(-3)(5)-(-6)(6)
\\
&=-15+36
\\
&=21.
\end{aligned}
$$

Both operations were row replacements, so the determinant remained unchanged at every step. Thus the original determinant is 21.

---

### Exercise 6. Parameter and Invertibility

**Problem**

For

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix}
$$

find all values of t for which the matrix is not invertible. Explain how the answer is related to the determinant being zero.

**Solution**

A square matrix is not invertible exactly when its determinant is zero.

Calculate the determinant:

$$
\det A(t)=t(t)-1(2)=t^2-2.
$$

Set the determinant equal to zero:

$$
t^2-2=0.
$$

Therefore,

$$
t^2=2
$$

and

$$
t=\sqrt{2}
\qquad\mathrm{or}\qquad
t=-\sqrt{2}.
$$

The matrix is not invertible for these two values. For every other real value of t, its determinant is nonzero and the matrix is invertible.

---

### Exercise 7. Using Properties Instead of Recomputing

**Problem**

Suppose that for a 3 × 3 matrix, the determinant of A is −4. Compute

$$
\det(2A),\qquad
\det(A^T),\qquad
\det(A^2),\qquad
\det(-A).
$$

Justify each answer using the appropriate property.

**Solution**

The given information is

$$
\det A=-4.
$$

**1. Determinant of 2A**

For an n × n matrix, multiplying every row by a scalar c multiplies the determinant by cⁿ. Since A is 3 × 3,

$$
\det(2A)=2^3\det A=8(-4)=-32.
$$

**2. Determinant of the transpose**

A matrix and its transpose have the same determinant:

$$
\det(A^T)=\det A=-4.
$$

**3. Determinant of A²**

The determinant of a product is the product of the determinants:

$$
\det(A^2)=\det(A)\det(A)=(-4)(-4)=16.
$$

**4. Determinant of −A**

Since A is 3 × 3, multiplying A by −1 multiplies its determinant by (−1)³:

$$
\det(-A)=(-1)^3\det A=(-1)(-4)=4.
$$

The four answers are therefore −32, −4, 16, and 4, respectively.

---

### Exercise 8. Determinant of a Product

**Problem**

Let A and B be square matrices such that the determinant of A is 3 and the determinant of B is −5. Compute

$$
\det(AB),\qquad
\det(BA)
$$

and, if it exists,

$$
\det(A^{-1}B).
$$

Explain why the first two results are equal even though AB is usually not equal to BA.

**Solution**

Use the product property:

$$
\det(AB)=\det A\det B.
$$

Therefore,

$$
\det(AB)=3(-5)=-15.
$$

Similarly,

$$
\det(BA)=\det B\det A=(-5)(3)=-15.
$$

The inverse A⁻¹ exists because det A = 3 is nonzero. The determinant of an inverse is the reciprocal of the original determinant:

$$
\det(A^{-1})=\frac{1}{\det A}=\frac{1}{3}.
$$

Thus,

$$
\begin{aligned}
\det(A^{-1}B)
&=\det(A^{-1})\det B
\\
&=\frac{1}{3}(-5)
\\
&=-\frac{5}{3}.
\end{aligned}
$$

The first two determinants are equal because multiplication of real numbers is commutative:

$$
\det A\det B=\det B\det A.
$$

This does not mean that AB = BA. The matrices themselves may be different even though their determinants are equal.

---

### Exercise 9. Area and the Determinant

**Problem**

The vectors

$$
u=
\begin{pmatrix}
3 \\
1
\end{pmatrix},
\qquad
v=
\begin{pmatrix}
1 \\
4
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

**Solution**

Place the two vectors as columns of a matrix:

$$
M=
\begin{pmatrix}
3 & 1 \\
1 & 4
\end{pmatrix}.
$$

The area of the parallelogram is the absolute value of the determinant:

$$
\begin{aligned}
\mathrm{Area}
&=|\det M|
\\
&=|3(4)-1(1)|
\\
&=|12-1|
\\
&=11.
\end{aligned}
$$

Now reverse the order of the vectors:

$$
N=
\begin{pmatrix}
1 & 3 \\
4 & 1
\end{pmatrix}.
$$

Swapping two columns changes the sign of the determinant. Direct calculation gives

$$
\det N=1(1)-3(4)=1-12=-11.
$$

The determinant changes from 11 to −11, but the area remains

$$
|\det N|=|-11|=11.
$$

The sign records orientation, while the absolute value gives the geometric area.

---

### Exercise 10. Detecting Dependence

**Problem**

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5
\end{pmatrix}
=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

**Solution**

The second row is exactly twice the first row:

$$
(2,4,6)=2(1,2,3).
$$

Therefore, the rows are linearly dependent. A square matrix with linearly dependent rows has determinant zero.

Consequently,

$$
\det A=0.
$$

A square matrix with determinant zero is not invertible. Thus the matrix is singular because one row is a multiple of another row.

---

## More Challenging Exercises

### Exercise 11. Shortening the Calculation with Row Operations

**Problem**

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

**Solution**

Start with

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}.
$$

Subtract the first row from the second row:

$$
R_2\leftarrow R_2-R_1.
$$

This row replacement does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 4 & 6
\end{pmatrix}.
$$

Subtract the first row from the third row:

$$
R_3\leftarrow R_3-R_1.
$$

This operation also does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3
\end{pmatrix}.
$$

Subtract twice the second row from the third row:

$$
R_3\leftarrow R_3-2R_2.
$$

This is another determinant-preserving row replacement:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}.
$$

The resulting matrix is upper triangular. Its determinant is the product of the diagonal entries:

$$
\det A=1(1)(1)=1.
$$

Every operation used was a row replacement, so none changed the determinant.

---

### Exercise 12. A Parameter Revealed by a Row Operation

**Problem**

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
$$

find the values of t for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2\leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter found.

**Solution**

Apply the required row operation:

$$
R_2\leftarrow R_2-2R_1.
$$

This operation does not change the determinant. The new second row is

$$
(2,4,t)-2(1,2,3)=(0,0,t-6).
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1
\end{pmatrix}.
$$

Expand along the first column, which contains two zeros below its first entry:

$$
\begin{aligned}
\det A(t)
&=
\begin{vmatrix}
0 & t-6 \\
1 & 1
\end{vmatrix}
\\
&=0(1)-(t-6)(1)
\\
&=6-t.
\end{aligned}
$$

The matrix is not invertible when its determinant is zero:

$$
6-t=0.
$$

Therefore,

$$
t=6.
$$

When t = 6, the original second row is

$$
(2,4,6)=2(1,2,3),
$$

so the second row is twice the first row. The rows are linearly dependent, which explains why the determinant is zero.

---

### Exercise 13. Determinant by Elimination

**Problem**

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

**Solution**

Use row replacements to obtain an upper triangular matrix. Each row replacement leaves the determinant unchanged.

Start with

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}.
$$

**Step 1.** Apply

$$
R_2\leftarrow R_2-2R_1.
$$

The determinant is unchanged:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2
\end{pmatrix}.
$$

**Step 2.** Apply

$$
R_3\leftarrow R_3-R_1.
$$

The determinant is unchanged again:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1
\end{pmatrix}.
$$

**Step 3.** Apply

$$
R_3\leftarrow R_3+2R_2.
$$

This row replacement also preserves the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}.
$$

The matrix is now upper triangular. Its determinant is

$$
\det A=1(1)(1)=1.
$$

No row swaps or row scalings were used. Every operation was a row replacement, so the determinant remained unchanged throughout the elimination.

---

### Exercise 14. A System of Equations and the Determinant

**Problem**

Consider the system Ax = b, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4
\end{pmatrix}.
$$

For which values of k does the system have exactly one solution for every b? For the remaining value, give an example of a right-hand side b for which there are infinitely many solutions, and an example for which there is no solution.

**Solution**

A 2 × 2 system has exactly one solution for every right-hand side b when its coefficient matrix is invertible. This happens when its determinant is nonzero.

Calculate the determinant:

$$
\det A=1(4)-2(k)=4-2k.
$$

For a unique solution for every b, require

$$
4-2k\neq 0.
$$

Therefore,

$$
k\neq 2.
$$

The exceptional value is k = 2. In that case,

$$
A=
\begin{pmatrix}
1 & 2 \\
2 & 4
\end{pmatrix}.
$$

The second row is twice the first row. The system becomes

$$
\begin{cases}
x+2y=b_1, \\
2x+4y=b_2.
\end{cases}
$$

**Example with infinitely many solutions**

Choose

$$
b=
\begin{pmatrix}
1 \\
2
\end{pmatrix}.
$$

The system is

$$
\begin{cases}
x+2y=1, \\
2x+4y=2.
\end{cases}
$$

The second equation is twice the first, so both equations describe the same line. There are infinitely many solutions. For example, all pairs satisfying x = 1 − 2y are solutions.

**Example with no solution**

Choose

$$
b=
\begin{pmatrix}
1 \\
3
\end{pmatrix}.
$$

The system is

$$
\begin{cases}
x+2y=1, \\
2x+4y=3.
\end{cases}
$$

Twice the first equation would give 2x + 4y = 2, but the second equation requires 2x + 4y = 3. These conditions contradict each other, so there is no solution.

Thus k = 2 is the only exceptional value: depending on b, the system has either infinitely many solutions or no solution.

---

### Exercise 15. Combining Determinant Properties

**Problem**

Let A and B be invertible 2 × 2 matrices with

$$
\det A=-2,
\qquad
\det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties used in order and explain why the factors involving B eventually cancel.

**Solution**

Use the determinant property for a product of square matrices:

$$
\det(XYZ)=\det X\det Y\det Z.
$$

Therefore,

$$
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B).
$$

The determinant of an inverse is the reciprocal of the determinant:

$$
\det(B^{-1})=\frac{1}{\det B}=\frac{1}{3}.
$$

A matrix and its transpose have the same determinant:

$$
\det(A^T)=\det A=-2.
$$

Substitute these values:

$$
\begin{aligned}
\det(B^{-1}A^TB)
&=\frac{1}{3}(-2)(3)
\\
&=-2.
\end{aligned}
$$

The factors involving B cancel because the determinant of B⁻¹ is the reciprocal of the determinant of B:

$$
\det(B^{-1})\det(B)=\frac{1}{3}(3)=1.
$$

The final result is therefore

$$
\det(B^{-1}A^TB)=-2.
$$
