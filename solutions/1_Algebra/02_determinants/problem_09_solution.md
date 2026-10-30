### Exercise 9. Area and the Determinant

**Problem**

The vectors

$$
u=
\begin{pmatrix}
3 \\
1
\end{pmatrix},
\qquad
v=
\begin{pmatrix}
1 \\
4
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

**Solution**

Place the two vectors as columns of a matrix:

$$
M=
\begin{pmatrix}
3 & 1 \\
1 & 4
\end{pmatrix}.
$$

The area of the parallelogram is the absolute value of the determinant:

$$
\begin{aligned}
\mathrm{Area}
&=|\det M|
\\
&=|3(4)-1(1)|
\\
&=|12-1|
\\
&=11.
\end{aligned}
$$

Now reverse the order of the vectors:

$$
N=
\begin{pmatrix}
1 & 3 \\
4 & 1
\end{pmatrix}.
$$

Swapping two columns changes the sign of the determinant. Direct calculation gives

$$
\det N=1(1)-3(4)=1-12=-11.
$$

The determinant changes from 11 to −11, but the area remains

$$
|\det N|=|-11|=11.
$$

The sign records orientation, while the absolute value gives the geometric area.

---
