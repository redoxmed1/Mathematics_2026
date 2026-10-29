### Exercise 7. Identity Matrix, Zero Matrix, and Powers

**Problem**

For

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix},
$$

compute AI, IA, A+0, A², and A³. Explain the roles of the identity matrix I and the zero matrix 0, and describe the pattern in successive powers of A.

**Solution**

For 2× 2 matrices, the identity and zero matrices are

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix},
\qquad
0=
\begin{pmatrix}
0 & 0 \\
0 & 0
\end{pmatrix}.
$$

**1. Identity products**

Multiplication by I leaves a matrix unchanged:

$$
AI=A,\qquad IA=A.
$$

Hence,

$$
AI=IA=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}.
$$

**2. Addition of the zero matrix**

Adding zero changes no entry:

$$
A+0=
\begin{pmatrix}
2+0 & 1+0 \\
0+0 & 2+0
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}.
$$

**3. Calculate A²**

$$
A^2=AA=
\begin{pmatrix}
2(2)+1(0) & 2(1)+1(2) \\
0(2)+2(0) & 0(1)+2(2)
\end{pmatrix}
=
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}.
$$

**4. Calculate A³**

$$
A^3=A^2A=
\begin{pmatrix}
4(2)+4(0) & 4(1)+4(2) \\
0(2)+4(0) & 0(1)+4(2)
\end{pmatrix}
=
\begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}.
$$

The identity matrix is the multiplicative identity, since multiplying by it leaves a matrix unchanged. The zero matrix is the additive identity, since adding it leaves a matrix unchanged. The diagonal entries of these powers are 2^n, while the top-right entries are n2^n-1 for the powers shown: 1, 4, 12. This pattern is consistent with the displayed values.

---
