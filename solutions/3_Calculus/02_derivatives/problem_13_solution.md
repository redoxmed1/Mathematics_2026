# Exercise 13: A Multi-Layer Composition

## Problem

For

$$
f(x)=e^{\sin(x^2)}
$$

compute the derivative. First write the layers

$$
x\longrightarrow x^2\longrightarrow \sin(x^2)\longrightarrow e^{\sin(x^2)}
$$

and explain why differentiation moves through them in the reverse order.

## Solution

### Step 1: Identify the layers

The given function is

$$
f(x)=e^{\sin(x^2)}.
$$

It contains three layers:

1. The innermost function:

$$
u(x)=x^2
$$

2. The middle function:

$$
v(u)=\sin u
$$

3. The outermost function:

$$
w(v)=e^v
$$

The composition is therefore

$$
x\longrightarrow x^2
\longrightarrow\sin(x^2)
\longrightarrow e^{\sin(x^2)}.
$$

### Step 2: Differentiate the innermost function

The innermost function is

$$
u(x)=x^2.
$$

Its derivative is

$$
\boxed{u'(x)=2x}
$$

### Step 3: Differentiate the middle function

The middle function is

$$
v(u)=\sin u.
$$

Its derivative with respect to $u$ is

$$
\frac{dv}{du}=\cos u.
$$

Substituting $u=x^2$:

$$
\frac{dv}{du}=\cos(x^2).
$$

### Step 4: Differentiate the outermost function

The outermost function is

$$
w(v)=e^v.
$$

Its derivative is

$$
\frac{dw}{dv}=e^v.
$$

Substituting $v=\sin(x^2)$:

$$
\frac{dw}{dv}=e^{\sin(x^2)}.
$$

### Step 5: Combine the derivatives

Using the chain rule, multiply the derivatives of the layers:

$$
f'(x)=
\frac{dw}{dv}
\cdot
\frac{dv}{du}
\cdot
\frac{du}{dx}.
$$

Substitute each expression:

$$
f'(x)=
e^{\sin(x^2)}
\cdot
\cos(x^2)
\cdot
2x.
$$

Therefore,

$$
\boxed{
f'(x)=2xe^{\sin(x^2)}\cos(x^2)
}
$$

### Step 6: Explain the reverse order

The original function is built from the inside outward:

$$
x\longrightarrow x^2
\longrightarrow\sin(x^2)
\longrightarrow e^{\sin(x^2)}.
$$

When differentiating, we begin with the outermost function and continue toward the innermost function.

This is why the chain rule multiplies the derivatives in the reverse order of the composition.

## Final Answer

$$
\boxed{
f'(x)=2xe^{\sin(x^2)}\cos(x^2)
}
$$
