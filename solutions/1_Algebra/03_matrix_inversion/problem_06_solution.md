
# Exercise 6 – Solving a System Using the Inverse

## Problem

Solve the matrix equation \(Ax=b\) using the inverse matrix method:

\[
A =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix},
\qquad
b =
\begin{pmatrix}
5 \\
7
\end{pmatrix}
\]

Use the formula:

\[
x=A^{-1}b
\]

Then substitute the resulting vector into the original equation to verify the answer.

---

## Solution

### 1. Calculate the determinant

First, calculate the determinant of matrix \(A\):

\[
\det(A)=2(3)-1(1)
\]

\[
\det(A)=6-1=5
\]

Since the determinant is not zero, matrix \(A\) is invertible.

### 2. Calculate the inverse matrix

For a \(2\times2\) matrix, the inverse formula is:

\[
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b\\
-c & a
\end{pmatrix}
\]

Substituting the values:

\[
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1\\
-1 & 2
\end{pmatrix}
\]

### 3. Find the solution using \(x=A^{-1}b\)

Multiply the inverse matrix by vector \(b\):

\[
x=
\frac{1}{5}
\begin{pmatrix}
3 & -1\\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
5\\
7
\end{pmatrix}
\]

Calculate each entry:

\[
x=
\frac{1}{5}
\begin{pmatrix}
3(5)-1(7)\\
-1(5)+2(7)
\end{pmatrix}
\]

\[
x=
\frac{1}{5}
\begin{pmatrix}
8\\
9
\end{pmatrix}
\]

Therefore, the solution is:

\[
\boxed{
x=
\begin{pmatrix}
\frac{8}{5}\\
\frac{9}{5}
\end{pmatrix}
}
\]

---

## Verification

To verify the solution, substitute the calculated vector into the original equation \(Ax=b\):

\[
\begin{pmatrix}
2 & 1\\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5}\\
\frac{9}{5}
\end{pmatrix}
=
\begin{pmatrix}
5\\
7
\end{pmatrix}
\]

Calculate each entry:

\[
=
\begin{pmatrix}
2(\frac{8}{5})+\frac{9}{5}\\
\frac{8}{5}+3(\frac{9}{5})
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
\frac{16}{5}+\frac{9}{5}\\
\frac{8}{5}+\frac{27}{5}
\end{pmatrix}
=
\begin{pmatrix}
\frac{25}{5}\\
\frac{35}{5}
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
5\\
7
\end{pmatrix}
=b
\]

The substitution gives the original vector \(b\), which confirms that the solution is correct.

---

## Final Answer

\[
\boxed{
x=
\begin{pmatrix}
\frac{8}{5}\\
\frac{9}{5}
\end{pmatrix}
}
\]

**Conclusion:** The system has a unique solution, and the verification confirms that the calculated vector is correct.
