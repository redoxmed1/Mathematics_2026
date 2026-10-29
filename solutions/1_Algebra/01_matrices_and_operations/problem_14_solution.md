### Exercise 14. Rotation Matrices

**Problem**

The matrix for a rotation through an angle θ is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}.
$$

Compute R(α)R(β) and, using the angle-sum formulas for sine and cosine, show that R(α)R(β)=R(α+β). Explain the result geometrically.

**Solution**

Write both matrices and multiply their rows by columns:

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta
\end{pmatrix}.
$$

The product is

$$
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta &
-\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta &
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}.
$$

Using the angle-sum identities

$$
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta
$$

and

$$
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta,
$$

the product becomes

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
=R(\alpha+\beta).
$$

Geometrically, rotating a vector by β and then by α is equivalent to one rotation by the combined angle α+β. The matrix calculation matches this geometric rule.

---
