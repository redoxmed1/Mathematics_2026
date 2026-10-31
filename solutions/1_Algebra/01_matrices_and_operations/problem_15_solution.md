### Exercise 15. Associativity of Multiplication and Different Calculation Paths

**Problem**

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix},
\qquad
C=
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix},
$$

compute (AB)C and A(BC).

Compare the results and the number of scalar multiplications
required by each calculation path.

Explain what associativity of matrix multiplication means
in this example.

**Solution**

**1. Check the dimensions**

The matrix dimensions are:

- A is 2 × 3.
- B is 3 × 2.
- C is 2 × 2.

Both calculation paths are possible.

For AB:

$$
(2 \times 3)(3 \times 2)=2 \times 2
$$

For BC:

$$
(3 \times 2)(2 \times 2)=3 \times 2
$$

Therefore, both final products have dimensions 2 × 2.

**2. First calculation path: (AB)C**

First calculate AB.

$$
AB=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
$$

Multiply rows by columns:

$$
AB=
\begin{pmatrix}
1(1)+2(2)+0(-1) & 1(0)+2(1)+0(3) \\
0(1)+1(2)+1(-1) & 0(0)+1(1)+1(3)
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
$$

Now multiply AB by C:

$$
(AB)C=
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
$$

$$
(AB)C=
\begin{pmatrix}
5(2)+2(0) & 5(1)+2(-1) \\
1(2)+4(0) & 1(1)+4(-1)
\end{pmatrix}
$$

$$
(AB)C=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
$$

**Scalar multiplication cost**

For multiplying an m × n matrix by an n × p matrix,
the number of scalar multiplications is m × n × p.

First multiplication, AB:

$$
2 \times 3 \times 2=12
$$

Second multiplication, (AB)C:

$$
2 \times 2 \times 2=8
$$

Total cost:

$$
12+8=20
$$

Therefore, the first calculation path requires 20 scalar multiplications.

**3. Second calculation path: A(BC)**

First calculate BC:

$$
BC=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
$$

Multiply rows by columns:

$$
BC=
\begin{pmatrix}
1(2)+0(0) & 1(1)+0(-1) \\
2(2)+1(0) & 2(1)+1(-1) \\
-1(2)+3(0) & -1(1)+3(-1)
\end{pmatrix}
$$

$$
BC=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
$$

Now multiply A by BC:

$$
A(BC)=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
$$

$$
A(BC)=
\begin{pmatrix}
1(2)+2(4)+0(-2) & 1(1)+2(1)+0(-4) \\
0(2)+1(4)+1(-2) & 0(1)+1(1)+1(-4)
\end{pmatrix}
$$

$$
A(BC)=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
$$

**Scalar multiplication cost**

First multiplication, BC:

$$
3 \times 2 \times 2=12
$$

Second multiplication, A(BC):

$$
2 \times 3 \times 2=12
$$

Total cost:

$$
12+12=24
$$

Therefore, the second calculation path requires 24 scalar multiplications.

**4. Compare the two calculation paths**

Both methods give the same final matrix:

$$
(AB)C=A(BC)=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
$$

However, their computational costs are different.

| Calculation path | Scalar multiplications |
|---|---:|
| (AB)C | 12 + 8 = 20 |
| A(BC) | 12 + 12 = 24 |

The first method is more efficient because it requires
20 scalar multiplications instead of 24.

The difference is:

$$
24-20=4
$$

Therefore, calculating (AB)C saves 4 scalar multiplications.

**Conclusion**

Associativity means that changing the grouping of three
compatible matrices does not change the final result:

$$
(AB)C=A(BC)
$$

However, the number of calculations can change depending
on the order of multiplication.

In this example, calculating AB first is more efficient
because it requires fewer scalar multiplications.
