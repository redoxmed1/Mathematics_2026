### Exercise 9. Composing Transformations

**Problem**

Let

$$
S=\begin{pmatrix}2&0\\0&1\end{pmatrix},\qquad
R=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
x=\begin{pmatrix}1\\2\end{pmatrix}.
$$

S describes horizontal scaling by 2, while R describes a 90° counterclockwise rotation. Compute RSx and SRx, compare the results, and explain why the order matters.

**Solution**

**Calculate RSx: scale first, then rotate.**

$$
Sx=\begin{pmatrix}2(1)+0(2)\\0(1)+1(2)\end{pmatrix}=\begin{pmatrix}2\\2\end{pmatrix}.
$$

Then calculate each row-by-column product for R(Sx):

$$
RSx=\begin{pmatrix}0(2)+(-1)(2)\\1(2)+0(2)\end{pmatrix}=\begin{pmatrix}-2\\2\end{pmatrix}.
$$

**Calculate SRx: rotate first, then scale.**

$$
Rx=\begin{pmatrix}0(1)+(-1)(2)\\1(1)+0(2)\end{pmatrix}=\begin{pmatrix}-2\\1\end{pmatrix}.
$$

Then apply S:

$$
SRx=\begin{pmatrix}2(-2)+0(1)\\0(-2)+1(1)\end{pmatrix}=\begin{pmatrix}-4\\1\end{pmatrix}.
$$

Thus,

$$
RSx=\begin{pmatrix}-2\\2\end{pmatrix},\qquad
SRx=\begin{pmatrix}-4\\1\end{pmatrix}.
$$

The results differ because S doubles only the horizontal coordinate. In RSx, the vector is scaled before it is rotated; in SRx, it is rotated first and the resulting horizontal coordinate is then doubled. The horizontal-only scaling therefore produces different final vectors depending on the order.
