### Exercise 7. Identity Matrix, Zero Matrix, and Powers

**Problem**

For

$$
A=\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix},
$$

compute AI, IA, A + 0, A², and A³. Explain the roles of I and 0, and describe the pattern in successive powers of A.

**Solution**

$$
I=\begin{pmatrix}1&0\\0&1\end{pmatrix},\qquad
0=\begin{pmatrix}0&0\\0&0\end{pmatrix}.
$$

Multiplication by the identity matrix and addition of the zero matrix leave A unchanged:

$$
AI=IA=A+0=\begin{pmatrix}2&1\\0&2\end{pmatrix}.
$$

**Calculate A² row by column.**

$$
A^2=\begin{pmatrix}
2(2)+1(0) & 2(1)+1(2) \\
0(2)+2(0) & 0(1)+2(2)
\end{pmatrix}
=\begin{pmatrix}4&4\\0&4\end{pmatrix}.
$$

**Calculate A³ row by column.**

$$
A^3=A^2A=\begin{pmatrix}
4(2)+4(0) & 4(1)+4(2) \\
0(2)+4(0) & 0(1)+4(2)
\end{pmatrix}
=\begin{pmatrix}8&12\\0&8\end{pmatrix}.
$$

The diagonal entries of Aⁿ are 2ⁿ. The upper-right entry follows the formula n·2ⁿ⁻¹, for n ≥ 1:

$$
A^n=\begin{pmatrix}
2^n & n2^{n-1} \\
0 & 2^n
\end{pmatrix},\qquad n\geq1.
$$

For n = 1, the upper-right entry is 1·2⁰ = 1; for n = 2 it is 2·2¹ = 4; for n = 3 it is 3·2² = 12. These values agree with A, A², and A³. The identity matrix is the multiplicative identity, while the zero matrix is the additive identity.
