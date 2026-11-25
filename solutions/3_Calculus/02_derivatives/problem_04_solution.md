# Exercise 4: A Quotient and Domain Control

## Problem

For

$$
f(x)=\frac{x^2+1}{x-1}
$$

determine the domain, compute the derivative, simplify the result, and explain why the restriction $x\neq1$ remains important.

## Solution

### Step 1: Determine the domain

The denominator cannot equal zero.

Therefore,

$$
x-1\neq0.
$$

Solving gives

$$
x\neq1.
$$

Thus, the domain is

$$
\boxed{D_f=\mathbb{R}\setminus\{1\}}
$$

### Step 2: Identify the numerator and denominator

We have

$$
u(x)=x^2+1
$$

and

$$
v(x)=x-1.
$$

Their derivatives are

$$
u'(x)=2x
$$

and

$$
v'(x)=1.
$$

### Step 3: Apply the quotient rule

The quotient rule is

$$
\left(\frac{u}{v}\right)'=
\frac{u'v-uv'}{v^2}.
$$

Substituting the expressions:

$$
f'(x)=\frac{2x(x-1)-(x^2+1)(1)}
{(x-1)^2}.
$$

### Step 4: Simplify the numerator

First, expand the multiplication:

$$
2x(x-1)=2x^2-2x.
$$

Therefore,

$$
f'(x)=\frac{2x^2-2x-(x^2+1)}
{(x-1)^2}.
$$

Remove the parentheses:

$$
f'(x)=\frac{2x^2-2x-x^2-1}
{(x-1)^2}.
$$

Combine like terms:

$$
\boxed{
f'(x)=\frac{x^2-2x-1}{(x-1)^2}
}
$$

### Step 5: Explain the domain restriction

The original function contains the denominator $x-1$.

At $x=1$, the denominator becomes zero, so the original function is undefined.

The derivative also contains the denominator $(x-1)^2$, which is zero at $x=1$.

Therefore, the restriction remains:

$$
x\neq1.
$$

The derivative is defined on the same domain:

$$
\boxed{D_{f'}=\mathbb{R}\setminus\{1\}}
$$

## Final Answer

The domain is

$$
\boxed{D_f=\mathbb{R}\setminus\{1\}}
$$

The derivative is

$$
\boxed{
f'(x)=\frac{x^2-2x-1}{(x-1)^2}
}
$$

The restriction $x\neq1$ is necessary because division by zero is not defined.
