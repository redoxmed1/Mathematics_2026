# Exercise 3: A Square Root and Removing an Indeterminate Form

## Problem

Compute

$$
\lim_{n\to\infty}\left(\sqrt{n^2+5n}-n\right).
$$

Use the conjugate expression and explain why this transformation removes the difficulty.

## Solution

Let

$$
L=\lim_{n\to\infty}\left(\sqrt{n^2+5n}-n\right).
$$

Direct substitution suggests an indeterminate form:

$$
\infty-\infty.
$$

We use the conjugate expression:

$$
\sqrt{n^2+5n}+n.
$$

Multiply and divide by this expression:

$$
L=\lim_{n\to\infty}
\frac{(\sqrt{n^2+5n}-n)(\sqrt{n^2+5n}+n)}
{\sqrt{n^2+5n}+n}.
$$

Using the identity

$$
(a-b)(a+b)=a^2-b^2,
$$

we obtain

$$
L=\lim_{n\to\infty}
\frac{n^2+5n-n^2}
{\sqrt{n^2+5n}+n}.
$$

Simplifying the numerator:

$$
L=\lim_{n\to\infty}
\frac{5n}{\sqrt{n^2+5n}+n}.
$$

Factor $n^2$ inside the square root:

$$
L=\lim_{n\to\infty}
\frac{5n}{n\sqrt{1+\frac{5}{n}}+n}.
$$

Since $n$ is positive, divide the numerator and denominator by $n$:

$$
L=\lim_{n\to\infty}
\frac{5}{\sqrt{1+\frac{5}{n}}+1}.
$$

Now,

$$
\frac{5}{n}\to0.
$$

Therefore,

$$
L=\frac{5}{\sqrt{1+0}+1}.
$$

$$
L=\frac{5}{1+1}.
$$

$$
\boxed{L=\frac52}
$$

## Explanation

The conjugate transformation changes the difference of two large expressions into a simpler fraction.

The identity

$$
(a-b)(a+b)=a^2-b^2
$$

allows us to cancel the terms $n^2$.

This removes the indeterminate form and makes the limit easy to calculate.

## Final Answer

$$
\boxed{\frac52}
$$
