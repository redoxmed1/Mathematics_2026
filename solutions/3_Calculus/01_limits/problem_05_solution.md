# Exercise 5: The Classical Limit Leading to the Number e

## Problem

Compute

$$
\lim_{n\to\infty}\left(1+\frac1n\right)^n.
$$

Calculate several values for increasing $n$ and compare the observed behavior with the value of the limit. Explain why a few values do not constitute a proof.

## Solution

The expression is a classical limit that defines the mathematical constant $e$:

$$
e=\lim_{n\to\infty}\left(1+\frac1n\right)^n.
$$

Therefore,

$$
\boxed{\lim_{n\to\infty}\left(1+\frac1n\right)^n=e}
$$

The approximate value is

$$
e\approx2.718281828.
$$

### Numerical Verification

We calculate several terms of the sequence.

For $n=1$:

$$
a_1=\left(1+\frac11\right)^1=2.
$$

For $n=2$:

$$
a_2=\left(1+\frac12\right)^2
=\left(\frac32\right)^2
=2.25.
$$

For $n=5$:

$$
a_5=\left(1+\frac15\right)^5
=(1.2)^5
\approx2.48832.
$$

For $n=10$:

$$
a_{10}=(1.1)^{10}\approx2.59374.
$$

For $n=100$:

$$
a_{100}=(1.01)^{100}\approx2.70481.
$$

For $n=1000$:

$$
a_{1000}=(1.001)^{1000}\approx2.71692.
$$

### Table of Values

| $n$ | Approximate value |
|---|---:|
| 1 | 2.00000 |
| 2 | 2.25000 |
| 5 | 2.48832 |
| 10 | 2.59374 |
| 100 | 2.70481 |
| 1000 | 2.71692 |

The values approach approximately 2.71828.

### Explanation

The numerical calculations support the conclusion that the sequence approaches $e$.

However, calculating a finite number of terms cannot prove that a sequence converges.

A mathematical proof must establish the behavior for all sufficiently large values of $n$, not just for the values calculated in a table.

## Final Answer

$$
\boxed{e\approx2.718281828}
$$
