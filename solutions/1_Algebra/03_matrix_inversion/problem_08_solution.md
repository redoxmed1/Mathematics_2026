### Exercise 8. Inverse of a Transformation

**Problem**

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12
\end{pmatrix}
$$

describes a scaling of the plane. Find S⁻¹ and explain geometrically what the inverse transformation does. Check the action of the pair S, S⁻¹ on one simple vector.

**Solution**

The matrix S doubles the horizontal coordinate and halves the vertical coordinate. To undo this transformation, the inverse must halve the horizontal coordinate and double the vertical coordinate.

Therefore,

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2
\end{pmatrix}.
$$

**Check using a vector**

Choose

$$
v=
\begin{pmatrix}
2 \\
4
\end{pmatrix}.
$$

Apply S:

$$
Sv=
\begin{pmatrix}
2(2)+0(4) \\
0(2)+\frac12(4)
\end{pmatrix}
=
\begin{pmatrix}
4 \\
2
\end{pmatrix}.
$$

Now apply S⁻¹ to the result:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac12(4)+0(2) \\
0(4)+2(2)
\end{pmatrix}
=
\begin{pmatrix}
2 \\
4
\end{pmatrix}
=v.
$$

The original vector is recovered. Geometrically, S⁻¹ undoes the nonuniform scaling performed by S.

---
