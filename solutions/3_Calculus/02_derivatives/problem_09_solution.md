# Exercise 9: A Logarithm and the Chain Rule

## Problem

For

$$
f(x)=\ln(x^2+1)
$$

compute the derivative. Then determine the sign of $f'(x)$ for $x<0$, $x=0$, and $x>0$, and describe qualitatively how the function behaves around zero.

## Solution

### Step 1: Identify the inner function

The given function is

$$
f(x)=\ln(x^2+1).
$$

The inner function is

$$
u(x)=x^2+1.
$$

Its derivative is

$$
u'(x)=2x.
$$

### Step 2: Apply the logarithmic derivative rule

The derivative of a natural logarithm is

$$
\frac{d}{dx}\ln(u(x))=\frac{u'(x)}{u(x)}.
$$

Substitute the inner function and its derivative:

$$
f'(x)=\frac{2x}{x^2+1}.
$$

Therefore,

$$
\boxed{f'(x)=\frac{2x}{x^2+1}}
$$

### Step 3: Determine the sign of the derivative

We examine the expression

$$
f'(x)=\frac{2x}{x^2+1}.
$$

The denominator is always positive because

$$
x^2\geq0
$$

and consequently

$$
x^2+1>0.
$$

Therefore, the sign of the derivative depends only on the numerator $2x$.

**Case 1: When $x<0$**

The numerator is negative, while the denominator is positive.

Thus,

$$
\boxed{f'(x)<0}
$$

The function is decreasing.

**Case 2: When $x=0$**

Substitute $x=0$:

$$
f'(0)=\frac{2(0)}{0^2+1}.
$$

$$
f'(0)=\frac01=0.
$$

Therefore,

$$
\boxed{f'(0)=0}
$$

**Case 3: When $x>0$**

The numerator is positive, and the denominator remains positive.

Thus,

$$
\boxed{f'(x)>0}
$$

The function is increasing.

### Step 4: Describe the behavior around zero

For negative values of $x$, the function decreases.

At $x=0$, the derivative equals zero.

For positive values of $x$, the function increases.

We can also calculate the function value at zero:

$$
f(0)=\ln(0^2+1).
$$

$$
f(0)=\ln1=0.
$$

Therefore, the function has a minimum at

$$
\boxed{(0,0)}
$$

The function decreases before zero and increases after zero.

## Final Answer

The derivative is

$$
\boxed{f'(x)=\frac{2x}{x^2+1}}
$$

Its sign is:

- $f'(x)<0$ for $x<0$.
- $f'(0)=0$.
- $f'(x)>0$ for $x>0$.

The function has a minimum at

$$
\boxed{(0,0)}
$$
