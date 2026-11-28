# Exercise 15 – Limits of a Sequence and a Function

## Problem

Study the following sequence and function.

**Part A – Sequence**

\[
a_n=\left(1+\frac{1}{n}\right)^n
\]

Calculate several terms of the sequence and determine its limit as \(n\) approaches infinity.

**Part B – Function**

\[
f(x)=\frac{x^2-4x+3}{x-3}
\]

Determine the limit as \(x\) approaches 3. Calculate the left-hand and right-hand limits, and explain the behaviour of the function near \(x=3\).

## Solution

# Part A – Sequence

### 1. Calculate the first terms

For \(n=1\):

\[
a_1=\left(1+\frac{1}{1}\right)^1=2
\]

For \(n=2\):

\[
a_2=\left(1+\frac{1}{2}\right)^2=2.25
\]

For \(n=5\):

\[
a_5=\left(1+\frac{1}{5}\right)^5\approx2.488320
\]

For \(n=10\):

\[
a_{10}=\left(1+\frac{1}{10}\right)^{10}\approx2.593742
\]

### 2. Numerical table

| \(n\) | \(a_n\) |
|---:|---:|
| 1 | 2.000000 |
| 2 | 2.250000 |
| 5 | 2.488320 |
| 10 | 2.593742 |
| 20 | 2.653298 |
| 50 | 2.691588 |
| 100 | 2.704814 |

The values increase and approach approximately 2.718282.

### 3. Limit of the sequence

The fundamental limit that defines Euler's number is:

\[
\boxed{\lim_{n\to\infty}\left(1+\frac{1}{n}\right)^n=e}
\]

where:

\[
e\approx2.718281828
\]

Therefore:

\[
\boxed{\lim_{n\to\infty}a_n=e}
\]

### 4. Graph of the sequence

![Graph of the sequence](images/exercise_15_sequence_graph.png)

The sequence consists of discrete points because \(n\) takes positive integer values. The connecting curve is only a visual guide.

### Conclusion for Part A

\[
\boxed{\lim_{n\to\infty}a_n=e\approx2.718282}
\]

# Part B – Function

### 1. Original function

\[
f(x)=\frac{x^2-4x+3}{x-3}
\]

We want to calculate:

\[
\lim_{x\to3}\frac{x^2-4x+3}{x-3}
\]

Direct substitution gives the indeterminate form:

\[
\frac{0}{0}
\]

Therefore, we need to simplify the expression.

### 2. Factorization

Factor the numerator:

\[
x^2-4x+3=(x-1)(x-3)
\]

Substitute this into the original function:

\[
f(x)=\frac{(x-1)(x-3)}{x-3}
\]

For \(x\neq3\), cancel the common factor:

\[
f(x)=x-1
\]

### 3. Calculate the two-sided limit

\[
\lim_{x\to3}(x-1)=3-1=2
\]

Therefore:

\[
\boxed{\lim_{x\to3}f(x)=2}
\]

### 4. Left-hand limit

\[
\lim_{x\to3^-}f(x)
=
\lim_{x\to3^-}(x-1)
=2
\]

Therefore:

\[
\boxed{\lim_{x\to3^-}f(x)=2}
\]

### 5. Right-hand limit

\[
\lim_{x\to3^+}f(x)
=
\lim_{x\to3^+}(x-1)
=2
\]

Therefore:

\[
\boxed{\lim_{x\to3^+}f(x)=2}
\]

### 6. Numerical verification

**Approaching 3 from the left:**

| \(x\) | \(f(x)=x-1\) |
|---:|---:|
| 2.9 | 1.9 |
| 2.99 | 1.99 |
| 2.999 | 1.999 |

**Approaching 3 from the right:**

| \(x\) | \(f(x)=x-1\) |
|---:|---:|
| 3.1 | 2.1 |
| 3.01 | 2.01 |
| 3.001 | 2.001 |

Both sides approach 2.

### 7. Graph and discontinuity

![Graph of the function](images/exercise_15_function_graph.png)

The graph is the straight line \(y=x-1\), with an open circle at \((3,2)\). The original function is undefined at \(x=3\), even though its limit exists and equals 2. This is a removable discontinuity.

### Final conclusion

The left-hand and right-hand limits are equal:

\[
\lim_{x\to3^-}f(x)=2
\]

\[
\lim_{x\to3^+}f(x)=2
\]

Therefore:

\[
\boxed{\lim_{x\to3}f(x)=2}
\]

## Final Summary

| Part | Result |
|---|---|
| Sequence limit | \(e\approx2.718282\) |
| Function left-hand limit | 2 |
| Function right-hand limit | 2 |
| Function two-sided limit | 2 |
| Discontinuity | Removable |
| Missing point | \((3,2)\) |
