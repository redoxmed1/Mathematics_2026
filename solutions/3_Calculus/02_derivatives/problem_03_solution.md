# Exercise 3: The Product Rule — Why Is It Needed?

## Problem

For

$$
f(x)=(x^2+1)e^x
$$

compute the derivative. Then compare the correct result with the incorrect idea

$$
f'(x)\stackrel{?}{=}(2x)e^x
$$

and explain which term is missing.

## Solution

### Step 1: Identify the two factors

The function is a product of two functions:

$$
u(x)=x^2+1
$$

and

$$
v(x)=e^x.
$$

Therefore,

$$
f(x)=u(x)v(x).
$$

We must use the product rule:

$$
(uv)'=u'v+uv'.
$$

### Step 2: Differentiate each factor

For the first factor:

$$
u(x)=x^2+1
$$

its derivative is

$$
u'(x)=2x.
$$

For the second factor:

$$
v(x)=e^x
$$

its derivative is

$$
v'(x)=e^x.
$$

### Step 3: Apply the product rule

Substitute the derivatives into the product rule:

$$
f'(x)=u'(x)v(x)+u(x)v'(x).
$$

Therefore,

$$
f'(x)=(2x)e^x+(x^2+1)e^x.
$$

Factor out the common factor $e^x$:

$$
f'(x)=e^x(2x+x^2+1).
$$

Rearranging the terms:

$$
\boxed{f'(x)=e^x(x^2+2x+1)}
$$

We can also write this as

$$
\boxed{f'(x)=e^x(x+1)^2}
$$

### Step 4: Compare with the incorrect result

The incorrect idea is

$$
f'(x)=(2x)e^x.
$$

This expression differentiates the first factor but does not differentiate the second factor.

The missing term is

$$
(x^2+1)e^x.
$$

The correct product rule requires both terms:

$$
f'(x)=(2x)e^x+(x^2+1)e^x.
$$

Therefore, differentiating only one factor is not sufficient.

## Final Answer

$$
\boxed{f'(x)=e^x(x+1)^2}
$$

The missing term in the incorrect result is

$$
\boxed{(x^2+1)e^x}
$$
