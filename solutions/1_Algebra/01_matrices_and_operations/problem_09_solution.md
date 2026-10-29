### Exercise 9. Composing Transformations

**Problem**

Let

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},
\qquad
R=
\begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}.
$$

The matrix S describes nonuniform scaling, while R describes a 90^\circ counterclockwise rotation. For

$$
x=
\begin{pmatrix}
1 \\
2
\end{pmatrix},
$$

compute RSx and SRx. Compare the results and explain geometrically why the order matters.

**Solution**

**1. Calculate RSx**

First apply S to x:

$$
Sx=
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\
2
\end{pmatrix}
=
\begin{pmatrix}
2 \\
2
\end{pmatrix}.
$$

Then rotate the result using R:

$$
RSx=
\begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
2 \\
2
\end{pmatrix}
=
\begin{pmatrix}
-2 \\
2
\end{pmatrix}.
$$

**2. Calculate SRx**

First rotate x:

$$
Rx=
\begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 \\
2
\end{pmatrix}
=
\begin{pmatrix}
-2 \\
1
\end{pmatrix}.
$$

Then apply the scaling:

$$
SRx=
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-2 \\
1
\end{pmatrix}
=
\begin{pmatrix}
-4 \\
1
\end{pmatrix}.
$$

The results are different:

$$
RSx=
\begin{pmatrix}-2\\2\end{pmatrix},
\qquad
SRx=
\begin{pmatrix}-4\\1\end{pmatrix}.
$$

Scaling first and then rotating is not the same as rotating first and then scaling. The scaling changes horizontal coordinates but not vertical coordinates, so changing when it is applied changes the final vector.

---
