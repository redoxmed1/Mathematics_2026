# Exercise 8: A Square Root in a Function Limit

## Problem

Compute

$$
\lim_{x\to4}\frac{\sqrt{x}-2}{x-4}
$$

by rationalizing the numerator. Compare the idea with Exercise 3 involving a sequence.

## Solution

Let

$$
L=\lim_{x\to4}\frac{\sqrt{x}-2}{x-4}.
$$

Direct substitution gives

$$
L=\frac{\sqrt4-2}{4-4}
=\frac{0}{0}.
$$

This is an indeterminate form.

We multiply the numerator and denominator by the conjugate of the numerator:

$$
\sqrt{x}+2.
$$

Thus,

$$
L=\lim_{x\to4}
\frac{(\sqrt{x}-2)(\sqrt{x}+2)}
{(x-4)(\sqrt{x}+2)}.
$$

Using the identity

$$
(a-b)(a+b)=a^2-b^2,
$$

we obtain

$$
L=\lim_{x\to4}
\frac{x-4}{(x-4)(\sqrt{x}+2)}.
$$

For $x\neq4$, cancel the common factor:

$$
L=\lim_{x\to4}\frac{1}{\sqrt{x}+2}.
$$

Now substitute $x=4$:

$$
L=\frac{1}{\sqrt4+2}.
$$

$$
L=\frac{1}{2+2}.
$$

$$
\boxed{L=\frac14}
$$

## Comparison with Exercise 3

In Exercise 3, we used the conjugate expression to simplify a sequence containing a square root.

Here, we use the same algebraic identity to simplify a function limit.

In both cases, multiplying by the conjugate removes an indeterminate form and makes the limit easier to calculate.

## Final Answer

$$
\boxed{\frac14}
$$
