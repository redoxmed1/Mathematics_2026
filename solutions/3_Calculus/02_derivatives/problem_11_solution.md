# Exercise 11: Derivative from the Definition

## Problem

Using only

$$
f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}h,
$$

find the derivative of $f(x)=x^2$. Compare the result with the power rule and indicate where the limit is used in the calculation.

## Solution

### Step 1: Write the definition of the derivative

We are given

$$
f(x)=x^2.
$$

Using the definition:

$$
f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}h.
$$

### Step 2: Calculate $f(x+h)$

Replace $x$ with $x+h$ in the original function:

$$
f(x+h)=(x+h)^2.
$$

Expand the square:

$$
(x+h)^2=x^2+2xh+h^2.
$$

Therefore,

$$
f(x+h)=x^2+2xh+h^2.
$$

### Step 3: Substitute into the definition

We have

$$
f'(x)=
\lim_{h\to0}
\frac{x^2+2xh+h^2-x^2}{h}.
$$

Cancel the terms $x^2$ and $-x^2$:

$$
f'(x)=
\lim_{h\to0}
\frac{2xh+h^2}{h}.
$$

### Step 4: Simplify the fraction

Factor out $h$ from the numerator:

$$
f'(x)=
\lim_{h\to0}
\frac{h(2x+h)}{h}.
$$

For $h\neq0$, cancel the common factor $h$:

$$
f'(x)=\lim_{h\to0}(2x+h).
$$

### Step 5: Evaluate the limit

Now let $h$ approach zero:

$$
f'(x)=2x+0.
$$

Therefore,

$$
\boxed{f'(x)=2x}
$$

### Step 6: Compare with the power rule

The power rule states

$$
\frac{d}{dx}(x^n)=nx^{n-1}.
$$

For $f(x)=x^2$, it gives

$$
f'(x)=2x^{2-1}.
$$

Thus,

$$
\boxed{f'(x)=2x}
$$

Both methods give the same result.

### Explanation

The limit is used after simplifying the difference quotient.

We cannot substitute $h=0$ at the beginning because the original expression would have a denominator equal to zero.

Instead, we first simplify the expression for $h\neq0$, and then calculate the limit as $h$ approaches zero.

## Final Answer

Using the definition of the derivative:

$$
\boxed{f'(x)=2x}
$$

This agrees with the result obtained using the power rule.
