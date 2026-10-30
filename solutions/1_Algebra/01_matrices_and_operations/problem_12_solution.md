### Exercise 12. Formula for a Matrix Power

**Problem**

Let

$$
A=\begin{pmatrix}1&1\\0&1\end{pmatrix}.
$$

Compute A², A³, and A⁴, conjecture a formula for Aⁿ, and prove the induction step by multiplying the proposed formula by A. Include the n = 0 case.

**Solution**

**Calculate A² row by column.**

$$
A^2=\begin{pmatrix}
1(1)+1(0) & 1(1)+1(1) \\
0(1)+1(0) & 0(1)+1(1)
\end{pmatrix}=\begin{pmatrix}1&2\\0&1\end{pmatrix}.
$$

**Calculate A³ row by column.**

$$
A^3=A^2A=\begin{pmatrix}
1(1)+2(0) & 1(1)+2(1) \\
0(1)+1(0) & 0(1)+1(1)
\end{pmatrix}=\begin{pmatrix}1&3\\0&1\end{pmatrix}.
$$

**Calculate A⁴ row by column.**

$$
A^4=A^3A=\begin{pmatrix}
1(1)+3(0) & 1(1)+3(1) \\
0(1)+1(0) & 0(1)+1(1)
\end{pmatrix}=\begin{pmatrix}1&4\\0&1\end{pmatrix}.
$$

The pattern suggests

$$
A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix},\qquad n\geq0.
$$

**Base case n = 0.** Since A⁰ = I,

$$
A^0=\begin{pmatrix}1&0\\0&1\end{pmatrix},
$$

which agrees with the formula when n = 0.

**Induction step.** Assume Aⁿ has the proposed form. Multiply Aⁿ by A and calculate each entry:

$$
A^{n+1}=A^nA=\begin{pmatrix}
1(1)+n(0) & 1(1)+n(1) \\
0(1)+1(0) & 0(1)+1(1)
\end{pmatrix}=\begin{pmatrix}1&n+1\\0&1\end{pmatrix}.
$$

This is exactly the proposed formula with n + 1 replacing n. The base case and induction step prove the formula for every nonnegative integer n.
