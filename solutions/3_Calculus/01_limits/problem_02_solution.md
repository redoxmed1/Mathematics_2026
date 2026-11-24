# Exercise 2: Different Growth Rates

## Problem

Compute

$$
\lim_{n\to\infty}\frac{3n+1}{n^2+4}
$$

and

$$
\lim_{n\to\infty}\frac{2n^3-n}{5n^2+1}.
$$

Compare the two cases and formulate a general observation about the degrees of the polynomials in the numerator and denominator.

## Solution

### Part 1

We calculate

$$
L_1=\lim_{n\to\infty}\frac{3n+1}{n^2+4}.
$$

The highest power in the denominator is $n^2$.

Divide every term by $n^2$:

$$
L_1=\lim_{n\to\infty}
\frac{\frac{3}{n}+\frac{1}{n^2}}
{1+\frac{4}{n^2}}.
$$

As $n\to\infty$,

$$
\frac{3}{n}\to0,\qquad
\frac{1}{n^2}\to0,\qquad
\frac{4}{n^2}\to0.
$$

Therefore,

$$
L_1=\frac{0+0}{1+0}.
$$

$$
\boxed{L_1=0}
$$

### Part 2

Now calculate

$$
L_2=\lim_{n\to\infty}\frac{2n^3-n}{5n^2+1}.
$$

Divide every term by $n^2$:

$$
L_2=\lim_{n\to\infty}
\frac{2n-\frac{1}{n}}
{5+\frac{1}{n^2}}.
$$

As $n\to\infty$,

$$
2n\to+\infty,
$$

$$
\frac{1}{n}\to0,
\qquad
\frac{1}{n^2}\to0.
$$

Thus,

$$
L_2=\frac{+\infty-0}{5+0}.
$$

Therefore,

$$
\boxed{L_2=+\infty}
$$

## Comparison and General Observation

The first limit equals zero because the denominator has a higher degree than the numerator.

The second limit equals positive infinity because the numerator has a higher degree than the denominator and its leading coefficient is positive.

For polynomial quotients:

- If the numerator has a smaller degree, the limit is zero.
- If both polynomials have the same degree, the limit is the ratio of their leading coefficients.
- If the numerator has a greater degree, the magnitude generally grows without bound. The sign depends on the leading terms.

## Final Answers

$$
\boxed{L_1=0}
$$

$$
\boxed{L_2=+\infty}
$$
