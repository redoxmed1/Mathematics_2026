# Exercise 12: Several Rules at Once

## Problem

For

$$
f(x)=(x^2+1)^3e^x
$$

compute the derivative. Before calculating, write down a plan: which rule applies to the whole expression and which rule applies to one of its factors. Finally, organize the result by factoring out common factors.

## Solution

### Step 1: Write a plan

The function is

$$
f(x)=(x^2+1)^3e^x.
$$

It is a product of two functions:

$$
u(x)=(x^2+1)^3
$$

and

$$
v(x)=e^x.
$$

Therefore, we use the product rule for the whole expression.

To differentiate $u(x)$, we use the chain rule because it contains a power of an inner function.

### Step 2: Differentiate the first factor

We have

$$
u(x)=(x^2+1)^3.
$$

Using the chain rule:

$$
u'(x)=3(x^2+1)^2\cdot\frac{d}{dx}(x^2+1).
$$

The derivative of the inner function is

$$
\frac{d}{dx}(x^2+1)=2x.
$$

Substitute:

$$
u'(x)=3(x^2+1)^2(2x).
$$

Simplifying:

$$
\boxed{u'(x)=6x(x^2+1)^2}
$$

### Step 3: Differentiate the second factor

The second factor is

$$
v(x)=e^x.
$$

Its derivative is

$$
\boxed{v'(x)=e^x}
$$

### Step 4: Apply the product rule

The product rule is

$$
(uv)'=u'v+uv'.
$$

Therefore,

$$
f'(x)=u'(x)v(x)+u(x)v'(x).
$$

Substitute the expressions:

$$
f'(x)=
6x(x^2+1)^2e^x
+
(x^2+1)^3e^x.
$$

### Step 5: Factor out the common factors

Both terms contain

$$
e^x(x^2+1)^2.
$$

Factor this expression out:

$$
f'(x)=
e^x(x^2+1)^2
\left[6x+(x^2+1)\right].
$$

Remove the parentheses:

$$
f'(x)=
e^x(x^2+1)^2
(6x+x^2+1).
$$

Rearranging:

$$
\boxed{
f'(x)=e^x(x^2+1)^2(x^2+6x+1)
}
$$

## Final Answer

The product rule is used for the whole expression, while the chain rule is used to differentiate the first factor.

The final derivative is

$$
\boxed{
f'(x)=e^x(x^2+1)^2(x^2+6x+1)
}
$$
