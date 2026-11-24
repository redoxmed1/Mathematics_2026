# Exercise 7: Limit at a Point and Canceling a Factor

## Problem

Compute

$$
\lim_{x\to3}\frac{x^2-4x+3}{x-3}.
$$

Explain why the value of the function at $x=3$ is not needed to compute the limit.

## Solution

Let

$$
L=\lim_{x\to3}\frac{x^2-4x+3}{x-3}.
$$

Direct substitution gives

$$
\frac{3^2-4(3)+3}{3-3}
=
\frac{9-12+3}{0}
=
\frac00.
$$

This is an indeterminate form.

We factorize the numerator:

$$
x^2-4x+3=(x-1)(x-3).
$$

Therefore,

$$
L=\lim_{x\to3}\frac{(x-1)(x-3)}{x-3}.
$$

For $x\neq3$, we can cancel the common factor:

$$
L=\lim_{x\to3}(x-1).
$$

Now substitute $x=3$:

$$
L=3-1.
$$

$$
\boxed{L=2}
$$

## Explanation

The original expression is undefined at $x=3$ because its denominator is zero.

However, the limit studies the behavior of the function when $x$ approaches 3, not necessarily the value of the function at 3.

For every $x$ close to 3 but different from 3, the simplified expression is equal to $x-1$.

Therefore, the limit exists even though the original function is undefined at that point.

## Final Answer

$$
\boxed{2}
$$
