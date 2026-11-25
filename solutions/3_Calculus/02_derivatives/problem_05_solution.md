# Exercise 5: The Chain Rule as Working Through Layers

## Problem

For

$$
f(x)=(3x^2-2x+1)^5
$$

identify the inner and outer functions, compute their derivatives, and combine the result according to the chain rule. Explain the origin of the additional factor.

## Solution

### Step 1: Identify the inner and outer functions

The function is

$$
f(x)=(3x^2-2x+1)^5.
$$

It is a composition of two functions.

The inner function is

$$
u(x)=3x^2-2x+1.
$$

The outer function is

$$
g(u)=u^5.
$$

Therefore,

$$
f(x)=g(u(x)).
$$

### Step 2: Differentiate the inner function

Differentiate

$$
u(x)=3x^2-2x+1.
$$

Using the power rule:

$$
u'(x)=3(2x)-2(1)+0.
$$

Simplifying:

$$
\boxed{u'(x)=6x-2}
$$

### Step 3: Differentiate the outer function

The outer function is

$$
g(u)=u^5.
$$

Its derivative is

$$
g'(u)=5u^4.
$$

### Step 4: Apply the chain rule

The chain rule states

$$
f'(x)=g'(u(x))\cdot u'(x).
$$

Substitute the expressions:

$$
f'(x)=5(3x^2-2x+1)^4(6x-2).
$$

Therefore,

$$
\boxed{
f'(x)=5(3x^2-2x+1)^4(6x-2)
}
$$

### Step 5: Explain the additional factor

The factor

$$
6x-2
$$

comes from differentiating the inner function.

We cannot differentiate only the outer power because the expression inside the parentheses also depends on $x$.

The chain rule requires us to multiply the derivative of the outer function by the derivative of the inner function.

## Final Answer

The inner function is

$$
u(x)=3x^2-2x+1
$$

The outer function is

$$
g(u)=u^5
$$

The derivative is

$$
\boxed{
f'(x)=5(3x^2-2x+1)^4(6x-2)
}
$$
