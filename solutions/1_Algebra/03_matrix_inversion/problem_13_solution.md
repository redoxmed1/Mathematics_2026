### Exercise 13. Undoing a Composite Transformation

**Problem**

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},
\qquad
H=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

describe nonuniform scaling and shear. For T = HS, find T⁻¹ in two ways:

1. first compute T, then its inverse,
2. use (HS)⁻¹ = S⁻¹H⁻¹.

Compare the results. Additionally compute H⁻¹S⁻¹ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

**Solution**

**Method 1. Calculate T first, then invert it**

Since T = HS,

$$
T=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1(2)+1(0) & 1(0)+1(1) \\
0(2)+1(0) & 0(0)+1(1)
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}.
$$

The determinant is 2(1) − 1(0) = 2. Therefore,

$$
T^{-1}
=
\frac12
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
$$

**Method 2. Reverse the order of the inverses**

First,

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix},
\qquad
H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}.
$$

Use the product inverse property:

$$
(HS)^{-1}=S^{-1}H^{-1}.
$$

Calculate:

$$
S^{-1}H^{-1}
=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
$$

Both methods give the same result:

$$
T^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
$$

**Check the incorrect order**

If the order is not reversed, the product is H⁻¹S⁻¹:

$$
H^{-1}S^{-1}
=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -1 \\
0 & 1
\end{pmatrix}.
$$

This is different from T⁻¹ because the upper-right entry is −1 instead of −1/2.

The transformation T = HS applies S first and then H. To undo the full transformation, H must be undone first, followed by S. Therefore, the inverse is S⁻¹H⁻¹: the order of operations is reversed.

---
