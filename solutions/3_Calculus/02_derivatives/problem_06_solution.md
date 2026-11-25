# Exercise 6: Product Rule and Trigonometry

## Problem

For

$$
f(x)=x\sin x+\cos x
$$

compute the derivative and simplify the result. Then compute $f'(0)$ and interpret the direction of the tangent line at that point.

## Solution

### Step 1: Identify the terms

The function is

$$
f(x)=x\sin x+\cos x.
$$

The first term is a product of two functions:

$$
u(x)=x
$$

and

$$
v(x)=\sin x.
$$

The second term is $\cos x$.

### Step 2: Differentiate the product

We use the product rule:

$$
(uv)'=u'v+uv'.
$$

The derivatives are

$$
u'(x)=1
$$

and

$$
v'(x)=\cos x.
$$

Therefore,

$$
\frac{d}{dx}(x\sin x)
=
1\cdot\sin x+x\cos x.
$$

Simplifying:

$$
\frac{d}{dx}(x\sin x)=\sin x+x\cos x.
$$

### Step 3: Differentiate the second term

We know that

$$
\frac{d}{dx}(\cos x)=-\sin x.
$$

### Step 4: Combine the derivatives

Therefore,

$$
f'(x)=\sin x+x\cos x-\sin x.
$$

The terms $\sin x$ and $-\sin x$ cancel:

$$
\boxed{f'(x)=x\cos x}
$$

### Step 5: Calculate $f'(0)$

Substitute $x=0$:

$$
f'(0)=0\cdot\cos0.
$$

Since

$$
\cos0=1,
$$

we obtain

$$
f'(0)=0\cdot1.
$$

Therefore,

$$
\boxed{f'(0)=0}
$$

### Step 6: Interpret the tangent direction

The derivative gives the slope of the tangent line.

Since the slope is zero, the tangent line is horizontal at $x=0$.

To identify the point of tangency, calculate

$$
f(0)=0\cdot\sin0+\cos0.
$$

$$
f(0)=0+1=1.
$$

Therefore, the point of tangency is $(0,1)$, and the tangent line is

$$
\boxed{y=1}
$$

## Final Answer

$$
\boxed{f'(x)=x\cos x}
$$

$$
\boxed{f'(0)=0}
$$

The tangent line at $(0,1)$ is horizontal:

$$
\boxed{y=1}
$$
