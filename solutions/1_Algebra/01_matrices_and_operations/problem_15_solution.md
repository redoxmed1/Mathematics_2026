### Exercise 15. Associativity of Multiplication and Different Calculation Paths

**Problem**

Given

$$
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},\quad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix},\quad
C=\begin{pmatrix}2&1\\0&-1\end{pmatrix},
$$

compute (AB)C and A(BC). Compare the results and the number of intermediate operations. Explain associativity.

**Solution**

The dimensions are compatible: A is 2 × 3, B is 3 × 2, and C is 2 × 2. Both paths are defined and produce a 2 × 2 matrix.

**1. Calculate (AB)C.** First calculate AB row by column:

$$
AB=\begin{pmatrix}
1(1)+2(2)+0(-1)&1(0)+2(1)+0(3)\\
0(1)+1(2)+1(-1)&0(0)+1(1)+1(3)
\end{pmatrix}=\begin{pmatrix}5&2\\1&4\end{pmatrix}.
$$

Now calculate (AB)C:

$$
(AB)C=\begin{pmatrix}
5(2)+2(0)&5(1)+2(-1)\\
1(2)+4(0)&1(1)+4(-1)
\end{pmatrix}=\begin{pmatrix}10&3\\2&-3\end{pmatrix}.
$$

**2. Calculate A(BC).** First calculate BC row by column:

$$
BC=\begin{pmatrix}
1(2)+0(0)&1(1)+0(-1)\\
2(2)+1(0)&2(1)+1(-1)\\
(-1)(2)+3(0)&(-1)(1)+3(-1)
\end{pmatrix}=\begin{pmatrix}2&1\\4&1\\-2&-4\end{pmatrix}.
$$

Now calculate A(BC):

$$
A(BC)=\begin{pmatrix}
1(2)+2(4)+0(-2)&1(1)+2(1)+0(-4)\\
0(2)+1(4)+1(-2)&0(1)+1(1)+1(-4)
\end{pmatrix}=\begin{pmatrix}10&3\\2&-3\end{pmatrix}.
$$

**3. Compare the paths.**

$$
(AB)C=A(BC)=\begin{pmatrix}10&3\\2&-3\end{pmatrix}.
$$

Each path uses two matrix multiplications: one intermediate multiplication and one final multiplication. The intermediate products differ: AB is 2 × 2, while BC is 3 × 2. Associativity means that changing only the grouping from (AB)C to A(BC) leaves the result unchanged. The factor order A, B, C stays the same; associativity does not mean that factors can be swapped.

