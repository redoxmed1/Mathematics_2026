# Exercise 2: Powers, Roots, and the Domain

## Problem

For

$$
f(x)=2\sqrt{x}-\frac{3}{x^2}+x^{3/2}
$$

1. Rewrite the function using powers.
2. Determine the domain.
3. Compute the derivative.
4. Compare the domain of the function with the domain of its derivative.

## Solution

### Step 1: Rewrite the function using powers

We use the following identities:

$$
\sqrt{x}=x^{1/2}
$$

and

$$
\frac{1}{x^2}=x^{-2}.
$$

Therefore, the original function becomes

$$
f(x)=2x^{1/2}-3x^{-2}+x^{3/2}.
$$

### Step 2: Determine the domain

We examine each term.

For the square root:

$$
\sqrt{x}
$$

we must have

$$
x\geq0.
$$

For the denominator:

$$
\frac{3}{x^2}
$$

we must have

$$
x\neq0.
$$

Combining these restrictions gives

$$
x>0.
$$

Therefore, the domain is

$$
\boxed{D_f=(0,+\infty)}
$$

### Step 3: Calculate the derivative

We use the power rule:

$$
\frac{d}{dx}(x^n)=nx^{n-1}.
$$

Starting with

$$
f(x)=2x^{1/2}-3x^{-2}+x^{3/2},
$$

differentiate each term.

For the first term:

$$
\frac{d}{dx}(2x^{1/2})=
2\cdot\frac12x^{-1/2}
$$

$$
=x^{-1/2}.
$$

For the second term:

$$
\frac{d}{dx}(-3x^{-2})=
-3(-2)x^{-3}
$$

$$
=6x^{-3}.
$$

For the third term:

$$
\frac{d}{dx}(x^{3/2})=
\frac32x^{1/2}.
$$

Combining the three derivatives:

$$
f'(x)=x^{-1/2}+6x^{-3}+\frac32x^{1/2}.
$$

Rewriting with positive exponents:

$$
\boxed{
f'(x)=\frac{1}{\sqrt{x}}+\frac{6}{x^3}+\frac32\sqrt{x}
}
$$

### Step 4: Compare the domains

The original function is defined for

$$
x>0.
$$

The derivative contains the terms

$$
\frac{1}{\sqrt{x}}
\quad\text{and}\quad
\frac{6}{x^3}.
$$

Both require $x>0$.

Therefore,

$$
D_{f'}=(0,+\infty).
$$

The two domains are equal:

$$
\boxed{D_f=D_{f'}=(0,+\infty)}
$$

## Final Answer

The function written using powers is

$$
f(x)=2x^{1/2}-3x^{-2}+x^{3/2}.
$$

Its domain is

$$
\boxed{D_f=(0,+\infty)}
$$

Its derivative is

$$
\boxed{
f'(x)=\frac{1}{\sqrt{x}}+\frac{6}{x^3}+\frac32\sqrt{x}
}
$$

The domain of the derivative is also

$$
\boxed{D_{f'}=(0,+\infty)}
$$
