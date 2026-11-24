# Exercise 1: Dominant Terms in a Sequence

## Problem

Compute

$$
\lim_{n\to\infty}\frac{4n^2-3n+1}{2n^2+5n-7}.
$$

Explain why the highest-degree terms determine the result.

## Solution

We start with

$$
L=\lim_{n\to\infty}\frac{4n^2-3n+1}{2n^2+5n-7}.
$$

The highest power of $n$ in both the numerator and denominator is $n^2$.

To simplify the expression, divide every term by $n^2$:

$$
L=\lim_{n\to\infty}
\frac{\frac{4n^2}{n^2}-\frac{3n}{n^2}+\frac{1}{n^2}}
{\frac{2n^2}{n^2}+\frac{5n}{n^2}-\frac{7}{n^2}}.
$$

Simplifying each term gives

$$
L=\lim_{n\to\infty}
\frac{4-\frac{3}{n}+\frac{1}{n^2}}
{2+\frac{5}{n}-\frac{7}{n^2}}.
$$

As $n$ approaches infinity,

$$
\lim_{n\to\infty}\frac{1}{n}=0
$$

and

$$
\lim_{n\to\infty}\frac{1}{n^2}=0.
$$

Therefore,

$$
L=\frac{4-0+0}{2+0-0}.
$$

$$
\boxed{L=2}
$$

## Explanation

The terms containing $n$ in the denominator approach zero as $n$ becomes very large.

Therefore, the highest-degree terms determine the limit.

In this example, the leading terms are $4n^2$ and $2n^2$, so the limit is their coefficient ratio:

$$
\frac{4}{2}=2.
$$

## Final Answer

$$
\boxed{2}
$$
