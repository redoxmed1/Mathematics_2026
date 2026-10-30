### Exercise 3. Swapping Two Rows

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
$$

compute the determinant. Then form a matrix B by swapping the first and second rows of A. First predict the determinant of B using a determinant property, and then verify the prediction by calculation.

**Solution**

First calculate the determinant of A by expanding along the first row:

$$
\begin{aligned}
\det A
&=1
\begin{vmatrix}
3 & 1 \\
1 & 1
\end{vmatrix}
-2
\begin{vmatrix}
0 & 1 \\
2 & 1
\end{vmatrix}
+0
\\
&=1(3(1)-1(1))-2(0(1)-1(2))
\\
&=2-2(-2)
\\
&=6.
\end{aligned}
$$

Swapping two rows changes the sign of a determinant. Therefore, before calculating B, the predicted value is

$$
\det B=-\det A=-6.
$$

After swapping the first and second rows,

$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}.
$$

Calculate its determinant by expanding along the first row:

$$
\begin{aligned}
\det B
&=0
-3
\begin{vmatrix}
1 & 0 \\
2 & 1
\end{vmatrix}
+1
\begin{vmatrix}
1 & 2 \\
2 & 1
\end{vmatrix}
\\
&=-3(1(1)-0(2))+(1(1)-2(2))
\\
&=-3-3
\\
&=-6.
\end{aligned}
$$

The direct calculation confirms the prediction: swapping two rows changes the determinant from 6 to −6.

---
