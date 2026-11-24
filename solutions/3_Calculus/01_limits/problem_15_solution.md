# Exercise 15: Observation Versus Proof

## Problem

Choose one sequence and one function from this set.

For the sequence, compute several values for increasingly large $n$.

For the function, prepare a table of values with arguments approaching the limit point from the left and right.

Sketch the behavior of both objects.

Compare the observation with the analytical result and explain why a finite number of calculations or a sketch does not constitute a proof that the limit exists.

## Solution

### Part 1: Sequence

We choose the sequence from Exercise 4:

$$
a_n=\left(\frac23\right)^n.
$$

We calculate several terms.

For $n=1$:

$$
a_1=\left(\frac23\right)^1
\approx0.666667.
$$

For $n=2$:

$$
a_2=\left(\frac23\right)^2
\approx0.444444.
$$

For $n=3$:

$$
a_3=\left(\frac23\right)^3
\approx0.296296.
$$

For $n=5$:

$$
a_5=\left(\frac23\right)^5
\approx0.131687.
$$

For $n=10$:

$$
a_{10}=\left(\frac23\right)^{10}
\approx0.017342.
$$

For $n=20$:

$$
a_{20}=\left(\frac23\right)^{20}
\approx0.000301.
$$

### Sequence Table

| $n$ | $a_n$ |
|---|---:|
| 1 | 0.666667 |
| 2 | 0.444444 |
| 3 | 0.296296 |
| 5 | 0.131687 |
| 10 | 0.017342 |
| 20 | 0.000301 |

The values become smaller and approach zero.

The analytical result is

$$
\lim_{n\to\infty}\left(\frac23\right)^n=0.
$$

### Part 2: Function

We choose the function from Exercise 7:

$$
f(x)=\frac{x^2-4x+3}{x-3}.
$$

For $x\neq3$, factorizing and simplifying gives

$$
f(x)=\frac{(x-1)(x-3)}{x-3}.
$$

Therefore,

$$
f(x)=x-1,\qquad x\neq3.
$$

We want to calculate

$$
\lim_{x\to3}f(x).
$$

### Table of Values

Approaching 3 from the left:

| $x$ | $f(x)=x-1$ |
|---|---:|
| 2.9 | 1.9 |
| 2.99 | 1.99 |
| 2.999 | 1.999 |

Approaching 3 from the right:

| $x$ | $f(x)=x-1$ |
|---|---:|
| 3.1 | 2.1 |
| 3.01 | 2.01 |
| 3.001 | 2.001 |

From both sides, the values approach 2.

Therefore,

$$
\boxed{\lim_{x\to3}f(x)=2}
$$

The original function is undefined at $x=3$, but this does not prevent the limit from existing.

### Part 3: Sketches

The sequence approaches zero:

```text
a_n
 |
0.7 | *
0.6 |
0.5 |    *
0.4 |
0.3 |       *
0.2 |           *
0.1 |                *
0.0 |________________________ n
       1  2  3  5  10  20
