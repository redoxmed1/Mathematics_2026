
# Exercise 8 – Inverse of a Transformation

## Problem

The following matrix describes a scaling transformation of the plane:

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

Find the inverse matrix S inverse and explain geometrically what the inverse transformation does. Check the action of S and its inverse on one simple vector.

---

## Solution

### Step 1: Understand the original transformation

The matrix S performs a nonuniform scaling of the plane.

- The horizontal coordinate (x) is multiplied by 2.
- The vertical coordinate (y) is multiplied by 1/2.

To undo this transformation, the inverse must:

- Divide the horizontal coordinate by 2.
- Multiply the vertical coordinate by 2.

### Step 2: Calculate the inverse transformation

The inverse transformation reverses the scaling performed by S.

Therefore, the inverse matrix is:

$$
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
$$

This matrix halves the horizontal coordinate and doubles the vertical coordinate.

### Step 3: Choose a vector for verification

Choose the following simple vector:

$$
v =
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

First, apply the original transformation S:

$$
Sv =
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

Calculate each entry:

$$
Sv =
\begin{pmatrix}
2(2)+0(4) \\
0(2)+\frac{1}{2}(4)
\end{pmatrix}
$$

Simplify:

$$
Sv =
\begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

### Step 4: Apply the inverse transformation

Now apply S inverse to the resulting vector:

$$
S^{-1}(Sv) =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

Calculate each entry:

$$
S^{-1}(Sv) =
\begin{pmatrix}
\frac{1}{2}(4)+0(2) \\
0(4)+2(2)
\end{pmatrix}
$$

Simplify:

$$
S^{-1}(Sv) =
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

Therefore:

$$
S^{-1}(Sv) = v
$$

The original vector is recovered, which confirms that the inverse transformation works correctly.

---

## Geometrical Explanation

The original transformation S stretches the plane horizontally by a factor of 2 and compresses it vertically by a factor of 1/2.

The inverse transformation S inverse does exactly the opposite:

- It compresses the plane horizontally by a factor of 1/2.
- It stretches the plane vertically by a factor of 2.

Applying both transformations in sequence returns every vector to its original position.

---

## Conclusion

The inverse matrix is:

$$
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
$$

The verification confirms that:

$$
S^{-1}(Sv) = v
$$

Therefore, the inverse transformation successfully reverses the original scaling.
