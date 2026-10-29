### Exercise 11. When Do Matrices Commute?

**Problem**

Given

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix},
$$

find the conditions on a,b,c,d under which AB=BA. Describe the general form of all such matrices B.

**Solution**

First calculate both products.

$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
=
\begin{pmatrix}
a+c & b+d \\
c & d
\end{pmatrix}.
$$

$$
BA=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
a & a+b \\
c & c+d
\end{pmatrix}.
$$

For AB=BA, corresponding entries must be equal. This gives

$$
a+c=a,\qquad b+d=a+b,\qquad c=c,\qquad d=c+d.
$$

The first equation gives c=0. The second gives d=a. The fourth also gives c=0, so it adds no new condition. There is no condition on b.

Thus, a and b may be any numbers, while c=0 and d=a. The general form is

$$
B=
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}.
$$

Substituting these conditions into both product formulas gives the same matrix, which verifies the result.

---
