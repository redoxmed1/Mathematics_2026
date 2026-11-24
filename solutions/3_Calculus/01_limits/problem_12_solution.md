# Exercise 12: Exponential Function Limit

## Problem

Compute

$$
\lim_{x\to0}(1+3x)^{1/x}.
$$

Connect the result with the limit from Exercise 5 and show the appropriate transformation.

## Solution

We start with

$$
L=\lim_{x\to0}(1+3x)^{1/x}.
$$

We want to use the classical limit

$$
\lim_{u\to0}(1+u)^{1/u}=e.
$$

Introduce the substitution

$$
u=3x.
$$

Then

$$
x=\frac{u}{3}
$$

and

$$
\frac1x=\frac3u.
$$

As $x\to0$, we also have $u\to0$.

Substituting gives

$$
L=\lim_{u\to0}(1+u)^{3/u}.
$$

Using the power rule,

$$
(1+u)^{3/u}
=
\left((1+u)^{1/u}\right)^3.
$$

Therefore,

$$
L=
\left(
\lim_{u\to0}(1+u)^{1/u}
\right)^3.
$$

Using the classical limit,

$$
L=e^3.
$$

Thus,

$$
\boxed{L=e^3}
$$

The approximate numerical value is

$$
e^3\approx20.0855.
$$

## Connection with Exercise 5

Exercise 5 introduced the classical limit

$$
\lim_{n\to\infty}\left(1+\frac1n\right)^n=e.
$$

The equivalent function limit is

$$
\lim_{u\to0}(1+u)^{1/u}=e.
$$

By substituting $u=3x$, we transform the given expression into the classical pattern.

## Final Answer

$$
\boxed{e^3\approx20.0855}
$$
