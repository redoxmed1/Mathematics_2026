# Exercise 8: Two Exponential Functions

## Problem

For

$$
f(x)=e^{2x-3}+5^x
$$

compute the derivative. Explain why the factor $2$ appears in the first term and why $\ln5$ appears in the second.

## Solution

### Step 1: Separate the two terms

The function is

$$
f(x)=e^{2x-3}+5^x.
$$

We differentiate each term separately using the sum rule.

### Step 2: Differentiate the first exponential term

Consider

$$
g(x)=e^{2x-3}.
$$

We use the chain rule.

The inner function is

$$
u(x)=2x-3.
$$

Its derivative is

$$
u'(x)=2.
$$

The derivative of the outer exponential function is

$$
\frac{d}{du}(e^u)=e^u.
$$

Applying the chain rule:

$$
g'(x)=e^{2x-3}\cdot2.
$$

Therefore,

$$
\boxed{g'(x)=2e^{2x-3}}
$$

The factor $2$ appears because the derivative of the exponent $2x-3$ is $2$.

### Step 3: Differentiate the second exponential term

Consider

$$
h(x)=5^x.
$$

We use the exponential derivative formula:

$$
\frac{d}{dx}(a^x)=a^x\ln a.
$$

For $a=5$:

$$
h'(x)=5^x\ln5.
$$

Therefore,

$$
\boxed{h'(x)=5^x\ln5}
$$

The factor $\ln5$ appears because the derivative of an exponential function with base $a$ is the original exponential function multiplied by $\ln a$.

### Step 4: Combine the derivatives

Using the sum rule:

$$
f'(x)=g'(x)+h'(x).
$$

Substituting the results:

$$
\boxed{
f'(x)=2e^{2x-3}+5^x\ln5
}
$$

## Final Answer

$$
\boxed{
f'(x)=2e^{2x-3}+5^x\ln5
}
$$

The factor $2$ comes from differentiating the exponent $2x-3$, while $\ln5$ comes from differentiating the exponential function with base 5.
