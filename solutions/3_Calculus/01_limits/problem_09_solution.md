# Exercise 9 – One-Sided Limits

## Problem

Consider the function:

$$
f(x)=\frac{1}{x-2}
$$

Study the left-hand and right-hand limits at $x=2$. Determine whether the two-sided limit exists. Identify the vertical and horizontal asymptotes, and sketch the graph.

## Solution

### 1. Domain of the function

The denominator must not be equal to zero:

$$
x-2\neq 0
$$

$$
x\neq 2
$$

Therefore, the domain is:

$$
\boxed{D_f=\mathbb{R}\setminus\{2\}}
$$

### 2. Left-hand limit

We calculate:

$$
\lim_{x\to 2^-}\frac{1}{x-2}
$$

When $x$ approaches 2 from the left, the denominator approaches zero through negative values. The numerator remains positive, so the quotient decreases without bound.

$$
\boxed{\lim_{x\to 2^-}\frac{1}{x-2}=-\infty}
$$

### 3. Right-hand limit

We calculate:

$$
\lim_{x\to 2^+}\frac{1}{x-2}
$$

When $x$ approaches 2 from the right, the denominator approaches zero through positive values. The quotient increases without bound.

$$
\boxed{\lim_{x\to 2^+}\frac{1}{x-2}=+\infty}
$$

### 4. Two-sided limit

The left-hand and right-hand limits are different. Therefore, the two-sided limit does not exist.

$$
\boxed{\lim_{x\to 2}f(x)\text{ does not exist}}
$$

### 5. Vertical asymptote

The function becomes unbounded as $x$ approaches 2. Thus, the vertical asymptote is:

$$
\boxed{x=2}
$$

### 6. Horizontal asymptote

As $x$ approaches positive or negative infinity, the function approaches zero:

$$
\lim_{x\to+\infty}\frac{1}{x-2}=0
$$

$$
\lim_{x\to-\infty}\frac{1}{x-2}=0
$$

Therefore, the horizontal asymptote is:

$$
\boxed{y=0}
$$

### 7. Graph

![Graph of Exercise 9](images/exercise_09_graph.png)

The dashed vertical line represents $x=2$, and the horizontal asymptote is $y=0$.

## Final Answer

- Domain: $\mathbb{R}\setminus\{2\}$
- Left-hand limit: $-\infty$
- Right-hand limit: $+\infty$
- Two-sided limit: Does not exist
- Vertical asymptote: $x=2$
- Horizontal asymptote: $y=0$
