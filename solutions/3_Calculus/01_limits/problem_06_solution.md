# Exercise 6: From a Sequence to a Function — Limit at Infinity

## Problem

Compute

$$
\lim_{x\to\infty}\frac{3x^2-x+1}{5x^2+4x-2}.
$$

Compare the method with Exercise 1. Explain what changes when moving from $n$ to a real variable $x$, and what stays the same.

## Solution

Let

$$
L=\lim_{x\to\infty}\frac{3x^2-x+1}{5x^2+4x-2}.
$$

The highest power in both the numerator and denominator is $x^2$.

Divide every term by $x^2$:

$$
L=\lim_{x\to\infty}
\frac{\frac{3x^2}{x^2}-\frac{x}{x^2}+\frac{1}{x^2}}
{\frac{5x^2}{x^2}+\frac{4x}{x^2}-\frac{2}{x^2}}.
$$

Simplifying gives

$$
L=\lim_{x\to\infty}
\frac{3-\frac1x+\frac1{x^2}}
{5+\frac4x-\frac2{x^2}}.
$$

As $x\to\infty$,

$$
\frac1x\to0
$$

and

$$
\frac1{x^2}\to0.
$$

Therefore,

$$
L=\frac{3-0+0}{5+0-0}.
$$

$$
\boxed{L=\frac35}
$$

## Comparison with Exercise 1

In Exercise 1, we calculated a limit involving the integer variable $n$.

Here, we calculate a limit involving the real variable $x$.

The main difference is that $n$ takes positive integer values, while $x$ can take any real value in its domain.

However, the algebraic method is the same: divide every term by the highest power of the variable.

In both exercises, the terms involving the reciprocal of the variable approach zero.

## Final Answer

$$
\boxed{\frac35}
$$
