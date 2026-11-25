# Exercise 14: Continuity and Differentiability of a Piecewise Function

## Problem

Investigate the behavior at $x=0$ of

$$
f(x)=
\begin{cases}
x^2, & x\geq0,\\
ax, & x<0.
\end{cases}
$$

For which values of $a$ is the function continuous? For which values do the one-sided derivatives exist and agree? For which value of $a$ is the function differentiable? Explain why continuity alone is not sufficient.

## Solution

### Step 1: Calculate the function value at zero

Since $0\geq0$, we use the first branch:

$$
f(0)=0^2.
$$

Therefore,

$$
\boxed{f(0)=0}
$$

### Step 2: Investigate continuity from the left

For $x<0$, the function is

$$
f(x)=ax.
$$

Calculate the left-hand limit:

$$
\lim_{x\to0^-}f(x)
=
\lim_{x\to0^-}ax.
$$

Since $a$ is a constant:

$$
\lim_{x\to0^-}f(x)
=
a\lim_{x\to0^-}x.
$$

Therefore,

$$
\boxed{\lim_{x\to0^-}f(x)=0}
$$

### Step 3: Investigate continuity from the right

For $x\geq0$, the function is

$$
f(x)=x^2.
$$

Calculate the right-hand limit:

$$
\lim_{x\to0^+}f(x)
=
\lim_{x\to0^+}x^2.
$$

Substituting zero:

$$
\boxed{\lim_{x\to0^+}f(x)=0}
$$

### Step 4: Determine the values of $a$ for continuity

A function is continuous at zero if

$$
\lim_{x\to0^-}f(x)
=
\lim_{x\to0^+}f(x)
=
f(0).
$$

We have found that

$$
\lim_{x\to0^-}f(x)=0,
$$

$$
\lim_{x\to0^+}f(x)=0,
$$

and

$$
f(0)=0.
$$

Therefore,

$$
0=0=0.
$$

This equality holds for every real value of $a$.

Thus, the function is continuous at zero for

$$
\boxed{a\in\mathbb{R}}
$$

### Step 5: Calculate the left-hand derivative

The left-hand derivative is defined by

$$
f'_-(0)=
\lim_{h\to0^-}
\frac{f(0+h)-f(0)}{h}.
$$

For $h<0$, we use the second branch:

$$
f(h)=ah.
$$

We also know that

$$
f(0)=0.
$$

Substitute:

$$
f'_-(0)=
\lim_{h\to0^-}
\frac{ah-0}{h}.
$$

Simplifying:

$$
f'_-(0)=
\lim_{h\to0^-}a.
$$

Therefore,

$$
\boxed{f'_-(0)=a}
$$

The left-hand derivative exists for every real value of $a$.

### Step 6: Calculate the right-hand derivative

The right-hand derivative is

$$
f'_+(0)=
\lim_{h\to0^+}
\frac{f(0+h)-f(0)}{h}.
$$

For $h>0$, we use the first branch:

$$
f(h)=h^2.
$$

Substitute:

$$
f'_+(0)=
\lim_{h\to0^+}
\frac{h^2-0}{h}.
$$

Simplifying:

$$
f'_+(0)=
\lim_{h\to0^+}h.
$$

Therefore,

$$
\boxed{f'_+(0)=0}
$$

The right-hand derivative also exists.

### Step 7: Determine when the function is differentiable

A function is differentiable at zero if the left-hand and right-hand derivatives exist and are equal.

We found

$$
f'_-(0)=a
$$

and

$$
f'_+(0)=0.
$$

Therefore, the condition is

$$
a=0.
$$

Thus,

$$
\boxed{a=0}
$$

is the only value for which the function is differentiable at zero.

### Step 8: Explain why continuity is not sufficient

Continuity only requires the function to approach the same value from the left and right.

Differentiability requires an additional condition: the left-hand and right-hand derivatives must also agree.

In this problem, the function is continuous for every real value of $a$, but it is differentiable only when $a=0$.

Therefore, continuity alone does not guarantee differentiability.

## Final Answer

The function is continuous at $x=0$ for every real value:

$$
\boxed{a\in\mathbb{R}}
$$

The one-sided derivatives are

$$
\boxed{f'_-(0)=a}
$$

and

$$
\boxed{f'_+(0)=0}
$$

The function is differentiable at zero only when

$$
\boxed{a=0}
$$
