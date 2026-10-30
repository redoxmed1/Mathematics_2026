### Exercise 8. Determinant of a Product

**Problem**

Let A and B be square matrices such that the determinant of A is 3 and the determinant of B is −5. Compute

$$
\det(AB),\qquad
\det(BA)
$$

and, if it exists,

$$
\det(A^{-1}B).
$$

Explain why the first two results are equal even though AB is usually not equal to BA.

**Solution**

Use the product property:

$$
\det(AB)=\det A\det B.
$$

Therefore,

$$
\det(AB)=3(-5)=-15.
$$

Similarly,

$$
\det(BA)=\det B\det A=(-5)(3)=-15.
$$

The inverse A⁻¹ exists because det A = 3 is nonzero. The determinant of an inverse is the reciprocal of the original determinant:

$$
\det(A^{-1})=\frac{1}{\det A}=\frac{1}{3}.
$$

Thus,

$$
\begin{aligned}
\det(A^{-1}B)
&=\det(A^{-1})\det B
\\
&=\frac{1}{3}(-5)
\\
&=-\frac{5}{3}.
\end{aligned}
$$

The first two determinants are equal because multiplication of real numbers is commutative:

$$
\det A\det B=\det B\det A.
$$

This does not mean that AB = BA. The matrices themselves may be different even though their determinants are equal.

---
