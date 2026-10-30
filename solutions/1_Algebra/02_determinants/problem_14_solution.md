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
