# Exercise 13: Fundamental Trigonometric Limit

## Problem

Using

$$
\lim_{x\to0}\frac{\sin x}{x}=1,
$$

compute

$$
\lim_{x\to0}\frac{\sin5x}{x}
$$

and

$$
\lim_{x\to0}\frac{\sin2x}{\sin3x}.
$$

In each case, show how you reduce the expression to the fundamental limit.

## Solution

We use the fundamental trigonometric limit:

$$
\lim_{u\to0}\frac{\sin u}{u}=1.
$$

### Part 1

Calculate

$$
L_1=\lim_{x\to0}\frac{\sin5x}{x}.
$$

Multiply and divide by 5:

$$
L_1=
\lim_{x\to0}
5\cdot\frac{\sin5x}{5x}.
$$

Rearrange:

$$
L_1=
5\lim_{x\to0}\frac{\sin5x}{5x}.
$$

Let

$$
u=5x.
$$

When $x\to0$, we have $u\to0$.

Using the fundamental limit:

$$
L_1=5\cdot1.
$$

Therefore,

$$
\boxed{L_1=5}
$$

### Part 2

Calculate

$$
L_2=\lim_{x\to0}\frac{\sin2x}{\sin3x}.
$$

Multiply and divide by the corresponding arguments:

$$
L_2=
\lim_{x\to0}
\frac{\sin2x}{2x}
\cdot
\frac{3x}{\sin3x}
\cdot
\frac23.
$$

Rearrange the factors:

$$
L_2=
\frac23
\lim_{x\to0}
\left(
\frac{\sin2x}{2x}
\cdot
\frac{3x}{\sin3x}
\right).
$$

Now use the fundamental limit:

$$
\lim_{x\to0}\frac{\sin2x}{2x}=1
$$

and

$$
\lim_{x\to0}\frac{3x}{\sin3x}=1.
$$

Therefore,

$$
L_2=\frac23\cdot1\cdot1.
$$

$$
\boxed{L_2=\frac23}
$$

## Final Answers

$$
\boxed{\lim_{x\to0}\frac{\sin5x}{x}=5}
$$

$$
\boxed{\lim_{x\to0}\frac{\sin2x}{\sin3x}=\frac23}
$$
