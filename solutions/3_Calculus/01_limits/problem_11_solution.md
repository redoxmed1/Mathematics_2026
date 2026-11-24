# Exercise 11: An n-th Root

## Problem

Compute

$$
\lim_{n\to\infty}\sqrt[n]{5^n+2^n}.
$$

Explain which term dominates and why the transformation looks different from the case of a quotient of polynomials.

## Solution

Let

$$
L=\lim_{n\to\infty}\sqrt[n]{5^n+2^n}.
$$

We factor out the largest exponential term, $5^n$:

$$
L=\lim_{n\to\infty}
\sqrt[n]{5^n\left(1+\frac{2^n}{5^n}\right)}.
$$

Simplifying the fraction inside the parentheses:

$$
L=\lim_{n\to\infty}
\sqrt[n]{5^n\left(1+\left(\frac25\right)^n\right)}.
$$

Using the property of roots,

$$
\sqrt[n]{ab}=\sqrt[n]{a}\sqrt[n]{b},
$$

we obtain

$$
L=\lim_{n\to\infty}
5\sqrt[n]{1+\left(\frac25\right)^n}.
$$

Since

$$
0<\frac25<1,
$$

we know that

$$
\lim_{n\to\infty}\left(\frac25\right)^n=0.
$$

Therefore,

$$
L=\lim_{n\to\infty}
5\sqrt[n]{1+\left(\frac25\right)^n}.
$$

The expression inside the root approaches 1. Hence,

$$
\lim_{n\to\infty}
\sqrt[n]{1+\left(\frac25\right)^n}=1.
$$

Thus,

$$
L=5\cdot1.
$$

$$
\boxed{L=5}
$$

## Explanation

The term $5^n$ dominates $2^n$ because 5 is greater than 2.

When we factor out $5^n$, the remaining exponential ratio is

$$
\left(\frac25\right)^n,
$$

which approaches zero.

Unlike a quotient of polynomials, this problem involves exponential terms and an n-th root. Therefore, we use the properties of roots and exponential expressions.

## Final Answer

$$
\boxed{5}
$$
