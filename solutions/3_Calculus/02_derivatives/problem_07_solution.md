# Exercise 7: A Trigonometric Composition

## Problem

For

$$
f(x)=\sin(x^2+1)
$$

compute the derivative. Explicitly identify the outer function, the inner function, and the derivative of the inner function. Finally, determine the sign of $f'(0)$.

## Solution

### Step 1: Identify the inner and outer functions

The given function is

$$
f(x)=\sin(x^2+1).
$$

The inner function is

$$
u(x)=x^2+1.
$$

The outer function is

$$
g(u)=\sin u.
$$

### Step 2: Differentiate the inner function

Using the power rule:

$$
u'(x)=2x+0.
$$

Therefore,

$$
\boxed{u'(x)=2x}
$$

### Step 3: Differentiate the outer function

We know that

$$
\frac{d}{du}(\sin u)=\cos u.
$$

Thus,

$$
g'(u)=\cos u.
$$

### Step 4: Apply the chain rule

The chain rule states

$$
f'(x)=g'(u(x))\cdot u'(x).
$$

Substituting the expressions:

$$
f'(x)=\cos(x^2+1)\cdot2x.
$$

Therefore,

$$
\boxed{f'(x)=2x\cos(x^2+1)}
$$

### Step 5: Determine the sign of $f'(0)$

Substitute $x=0$:

$$
f'(0)=2(0)\cos(0^2+1).
$$

Simplifying:

$$
f'(0)=0\cdot\cos1.
$$

Therefore,

$$
\boxed{f'(0)=0}
$$

The derivative is neither positive nor negative at this point; it equals zero.

Consequently, the tangent line at $x=0$ is horizontal.

## Final Answer

Inner function:

$$
\boxed{u(x)=x^2+1}
$$

Outer function:

$$
\boxed{g(u)=\sin u}
$$

Derivative:

$$
\boxed{f'(x)=2x\cos(x^2+1)}
$$

At $x=0$:

$$
\boxed{f'(0)=0}
$$
