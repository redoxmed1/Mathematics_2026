# Exercise 13 – Undoing a Composite Transformation

## Problem

The matrices

$$S = \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix}, \qquad H = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}$$

describe non-uniform scaling and shear. For $T = HS$, find $T^{-1}$ in two ways:

1. First compute $T$, then compute its inverse.
2. Use the product inverse property $(HS)^{-1} = S^{-1}H^{-1}$.

Compare the results. Additionally, compute $H^{-1}S^{-1}$ and verify that using the incorrect order gives a different matrix. Explain the general rule: *"when undoing a composition of operations, we must undo them in reverse order."*

---

## Solution

### Step 1: Compute T = HS and find its inverse directly (Method 1)

#### Calculate $T$
Multiply matrix $H$ by matrix $S$:

$$T = HS = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix}$$

Calculate each entry:

$$T = \begin{pmatrix} (1)(2) + (1)(0) & (1)(0) + (1)(1) \\\\ (0)(2) + (1)(0) & (0)(0) + (1)(1) \end{pmatrix}$$

$$T = \begin{pmatrix} 2 & 1 \\\\ 0 & 1 \end{pmatrix}$$

#### Calculate $T^{-1}$
Find the determinant of $T$:

$$\det(T) = (2)(1) - (1)(0) = 2$$

Apply the $2 \times 2$ inverse formula:

$$T^{-1} = \frac{1}{2} \begin{pmatrix} 1 & -1 \\\\ 0 & 2 \end{pmatrix}$$

$$T^{-1} = \begin{pmatrix} \frac{1}{2} & -\frac{1}{2} \\\\ 0 & 1 \end{pmatrix}$$

---

### Step 2: Find T⁻¹ using the product inverse property (Method 2)

#### Find individual inverses $S^{-1}$ and $H^{-1}$
For diagonal matrix $S$:

$$S^{-1} = \begin{pmatrix} \frac{1}{2} & 0 \\\\ 0 & 1 \end{pmatrix}$$

For shear matrix $H$:

$$\det(H) = (1)(1) - (1)(0) = 1 \implies H^{-1} = \begin{pmatrix} 1 & -1 \\\\ 0 & 1 \end{pmatrix}$$

#### Apply property $(HS)^{-1} = S^{-1}H^{-1}$
Multiply $S^{-1}$ by $H^{-1}$:

$$(HS)^{-1} = S^{-1}H^{-1} = \begin{pmatrix} \frac{1}{2} & 0 \\\\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & -1 \\\\ 0 & 1 \end{pmatrix}$$

Calculate each entry:

$$S^{-1}H^{-1} = \begin{pmatrix} \left(\frac{1}{2}\right)(1) + (0)(0) & \left(\frac{1}{2}\right)(-1) + (0)(1) \\\\ (0)(1) + (1)(0) & (0)(-1) + (1)(1) \end{pmatrix}$$

Simplify:

$$S^{-1}H^{-1} = \begin{pmatrix} \frac{1}{2} & -\frac{1}{2} \\\\ 0 & 1 \end{pmatrix}$$

Both methods yield the exact same inverse matrix $T^{-1}$.

---

### Step 3: Check the incorrect order H⁻¹S⁻¹

Compute the product without reversing the order of inverses:

$$H^{-1}S^{-1} = \begin{pmatrix} 1 & -1 \\\\ 0 & 1 \end{pmatrix} \begin{pmatrix} \frac{1}{2} & 0 \\\\ 0 & 1 \end{pmatrix}$$

Calculate each entry:

$$H^{-1}S^{-1} = \begin{pmatrix} (1)\left(\frac{1}{2}\right) + (-1)(0) & (1)(0) + (-1)(1) \\\\ (0)\left(\frac{1}{2}\right) + (1)(0) & (0)(0) + (1)(1) \end{pmatrix}$$

Simplify:

$$H^{-1}S^{-1} = \begin{pmatrix} \frac{1}{2} & -1 \\\\ 0 & 1 \end{pmatrix}$$

#### Comparison
$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\\\
0 & 1
\end{pmatrix}
\neq
\begin{pmatrix}
\frac{1}{2} & -1 \\\\
0 & 
