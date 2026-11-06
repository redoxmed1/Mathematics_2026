# Exercise 13 – Undoing a Composite Transformation

## Problem

The matrices

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},
\qquad
H =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

describe non-uniform scaling and shear. For $T = HS$, find $T^{-1}$ in two ways:

1. First compute $T$, then compute its inverse.
2. Use the product inverse property $(HS)^{-1} = S^{-1}H^{-1}$.

Compare the results. Additionally, compute $H^{-1}S^{-1}$ and verify that using the incorrect order gives a different matrix. Explain the general rule: *"when undoing a composition of operations, we must undo them in reverse order."*

---

## Solution

### Step 1: Compute T = HS and find its inverse directly (Method 1)

#### Calculate $T$
Multiply matrix $H$ by matrix $S$:

$$
T = HS =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

Calculate each entry:

$$
T =
\begin{pmatrix}
(1)(2) + (1)(0) & (1)(0) + (1)(1) \\
(0)(2) + (1)(0) & (0)(0) + (1)(1)
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}
$$

#### Calculate $T^{-1}$
Find the determinant of $T$:

$$
\det(T) = (2)(1) - (1)(0) = 2
$$

Apply the $2 \times 2$ inverse formula:

$$
T^{-1} = \frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

---

### Step 2: Find T⁻¹ using the product inverse property (Method 2)

#### Find individual inverses $S^{-1}$ and $H^{-1}$
For diagonal matrix $S$:

$$
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
$$

For shear matrix $H$:

$$
\det(H) = (1)(1) - (1)(0) = 1 \implies H^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

#### Apply property $(HS)^{-1} = S^{-1}H^{-1}$
Multiply $S^{-1}$ by $H^{-1}$:

$$
(HS)^{-1} = S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Calculate each entry:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\left(\frac{1}{2}\right)(1) + (0)(0) & \left(\frac{1}{2}\right)(-1) + (0)(1) \\
(0)(1) + (1)(0) & (0)(-1) + (1)(1)
\end{pmatrix}
$$

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

Both methods yield the exact same inverse matrix $T^{-1}$.

---

### Step 3: Check the incorrect order H⁻¹S⁻¹

Compute the product without reversing the order of inverses:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
$$

Calculate each entry:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
(1)\left(\frac{1}{2}\right) + (-1)(0) & (1)(0) + (-1)(1) \\
(0)\left(\frac{1}{2}\right) + (1)(0) & (0)(0) + (1)(1)
\end{pmatrix}
=
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
$$

#### Comparison
$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
\neq
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
= H^{-1}S^{-1}
$$

The upper-right entry is $-\frac{1}{2}$ for $T^{-1}$, whereas $H^{-1}S^{-1}$ yields $-1$. Thus, $H^{-1}S^{-1} \neq T^{-1}$.

---

### Step 4: Conceptual explanation of the order rule

When a vector $\mathbf{x}$ is transformed by $T = HS$, the operations occur sequentially:

1. Matrix $S$ acts on $\mathbf{x}$ **first**: $\mathbf{y} = S\mathbf{x}$.
2. Matrix $H$ acts on the result **second**: $T\mathbf{x} = H(S\mathbf{x})$.

To undo (reverse) this transformation step-by-step:

1. We must undo the last operation $H$ **first** by applying $H^{-1}$.
2. We then undo the initial operation $S$ **second** by applying $S^{-1}$.

Algebraically:

$$
(HS)^{-1} (HS) = S^{-1} (H^{-1} H) S = S^{-1} I S = S^{-1} S = I
$$

This explains why matrix multiplication order reverses when taking the inverse of a composition: $(AB)^{-1} = B^{-1}A^{-1}$.

---

## Conclusion

- **Direct Computation (Method 1):**

$$
T^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

- **Product Property (Method 2):**

$$
(HS)^{-1} = S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

- **Incorrect Order:**

$$
H^{-1}S^{-1} =
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
\neq T^{-1}
$$

The inverse of a composite transformation $(HS)^{-1}$ requires reversing the operational sequence to $S^{-1}H^{-1}$.
