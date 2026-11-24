# Exercise 4: Powers and Oscillation

## Problem

Analyze the following sequences:

$$
\left(\frac23\right)^n,\qquad
\left(\frac32\right)^n,\qquad
(-1)^n,\qquad
\frac{(-1)^n}{n}.
$$

For each sequence, describe its behavior and justify your answer.

## Solution

### Part 1

Consider

$$
a_n=\left(\frac23\right)^n.
$$

The base satisfies

$$
0<\frac23<1.
$$

A positive number smaller than 1 approaches zero when raised to increasingly large powers.

Therefore,

$$
\boxed{\lim_{n\to\infty}\left(\frac23\right)^n=0}
$$

This sequence is convergent.

### Part 2

Consider

$$
b_n=\left(\frac32\right)^n.
$$

The base satisfies

$$
\frac32>1.
$$

Powers of a number greater than 1 increase without bound.

Therefore,

$$
\boxed{\lim_{n\to\infty}\left(\frac32\right)^n=+\infty}
$$

This sequence diverges to positive infinity.

### Part 3

Consider

$$
c_n=(-1)^n.
$$

The terms alternate between $-1$ and $1$:

$$
-1,\ 1,\ -1,\ 1,\ldots
$$

The even-indexed terms equal 1, while the odd-indexed terms equal -1.

Since the sequence does not approach one unique value, its limit does not exist.

$$
\boxed{\lim_{n\to\infty}(-1)^n\text{ does not exist}}
$$

This sequence oscillates.

### Part 4

Consider

$$
d_n=\frac{(-1)^n}{n}.
$$

The absolute value is

$$
|d_n|=\frac{1}{n}.
$$

Since

$$
\lim_{n\to\infty}\frac1n=0,
$$

the absolute value of the sequence approaches zero.

By the squeeze theorem,

$$
-\frac1n\leq\frac{(-1)^n}{n}\leq\frac1n.
$$

Both bounds approach zero. Therefore,

$$
\boxed{\lim_{n\to\infty}\frac{(-1)^n}{n}=0}
$$

This sequence oscillates, but its oscillations become smaller and smaller.

## Final Answers

1. $\left(\frac23\right)^n$ converges to 0.
2. $\left(\frac32\right)^n$ diverges to positive infinity.
3. $(-1)^n$ oscillates and has no limit.
4. $\frac{(-1)^n}{n}$ oscillates but converges to 0.
