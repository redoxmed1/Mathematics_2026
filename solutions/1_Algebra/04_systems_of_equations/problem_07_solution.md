### Exercise 7. Choosing a Method Deliberately

**Problem**

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. One system with a triangular coefficient matrix:

$$
\begin{cases}
2x-y=3,\\
4y=8.
\end{cases}
$$

2. Three systems Ax = bᵢ with the same invertible matrix A, when A⁻¹ is already known.

3. One 3×3 system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

**Solution**

**Step 1. Case 1 — Triangular System**

The given system is:

$$
\begin{cases}
2x-y=3,\\
4y=8.
\end{cases}
$$

Since the system has a triangular structure, the best method is back substitution.

First, solve the second equation:

$$
4y=8
$$

Divide both sides by 4:

$$
y=\frac{8}{4}=2
$$

Now substitute y = 2 into the first equation:

$$
2x-y=3
$$

$$
2x-2=3
$$

Add 2 to both sides:

$$
2x=5
$$

Divide both sides by 2:

$$
x=\frac{5}{2}
$$

Therefore, the solution is:

$$
\boxed{x=\frac{5}{2},\quad y=2}
$$

**Step 2. Verify the Solution**

First equation:

$$
2x-y=3
$$

Substitute the values:

$$
2\left(\frac{5}{2}\right)-2=3
$$

$$
5-2=3
$$

$$
3=3
$$

Second equation:

$$
4y=8
$$

$$
4(2)=8
$$

$$
8=8
$$

Both equations are satisfied.

Therefore, the solution is correct.

**Step 3. Case 2 — Three Systems with the Same Invertible Matrix**

In this situation, we have three systems:

$$
Ax=b_1,\qquad Ax=b_2,\qquad Ax=b_3
$$

All three systems have the same invertible coefficient matrix A, and its inverse A⁻¹ is already known.

The best method is to use the inverse matrix.

For each system, multiply both sides by A⁻¹:

$$
x_1=A^{-1}b_1
$$

$$
x_2=A^{-1}b_2
$$

$$
x_3=A^{-1}b_3
$$

The main advantage is that the inverse matrix only needs to be calculated once because A is the same in all three systems.

We can reuse A⁻¹ for all three calculations.

There is no need to calculate the inverse again or repeat the entire elimination process for each system.

Only the multiplication with each different right-hand side is necessary.

Therefore, using the known inverse is an efficient method when several systems share the same invertible coefficient matrix.

**Step 4. Case 3 — One 3×3 System with One Solution Vector**

In this situation, we have one 3×3 system, the inverse matrix is not given, and we only need to find one solution vector.

The best method is Gaussian elimination.

We can write the system as an augmented matrix:

$$
[A\mid b]
$$

Then, use elementary row operations to transform the matrix into row echelon form or reduced row echelon form.

After that, we can use back substitution or read the solution directly to find the unknown variables.

Gaussian elimination is more appropriate here because we only need one solution vector.

Calculating the entire inverse matrix would require additional unnecessary work.

There is no advantage in finding all the entries of A⁻¹ when we only need to solve one system.

Therefore, Gaussian elimination is the more efficient choice for this situation.

**Step 5. Comparison of the Three Cases**

The best method depends on the structure of the system and how many right-hand sides we need to solve.

- Case 1: Back substitution is the best choice because the coefficient matrix has a triangular structure. We can solve the system directly without unnecessary calculations.

- Case 2: Using the inverse matrix is efficient because the same invertible matrix is used in three systems, and its inverse is already known. The inverse can be reused for all three right-hand sides.

- Case 3: Gaussian elimination is the best choice because we only need one solution vector and the inverse matrix is not given. Calculating the full inverse would require unnecessary computations.

**Conclusion**

These three situations show that there is no single method that is always the best for solving systems of linear equations.

The choice depends on the structure of the coefficient matrix, whether the inverse is already available, and the number of systems that must be solved.

Back substitution is efficient for triangular systems, using an existing inverse is useful for multiple right-hand sides, and Gaussian elimination is preferable when solving one system without needing the inverse matrix.

The most efficient method is the one that avoids unnecessary calculations while solving the problem correctly.
