# Exercise 15: The Difference Quotient as a Check of the Derivative

## Problem

Choose one function from the problem set and a point $x_0$ at which the derivative exists. Compute $f'(x_0)$ exactly, and then calculate

$$
\frac{f(x_0+h)-f(x_0)}h
$$

for $h=1$, $0.1$, and $0.01$. Compare the values with $f'(x_0)$ and explain why the difference quotient approaching a single number is consistent with the definition of the derivative, while a few computations do not replace a limit argument.

## Solution

### Step 1: Choose a function and a point

We choose the function from Exercise 11:

$$
f(x)=x^2.
$$

We choose the point

$$
x_0=1.
$$

The function is differentiable at this point.

### Step 2: Calculate the exact derivative

Using the power rule:

$$
f'(x)=2x.
$$

Substitute $x_0=1$:

$$
f'(1)=2(1).
$$

Therefore,

$$
\boxed{f'(1)=2}
$$

### Step 3: Calculate the difference quotient

The difference quotient is

$$
\frac{f(x_0+h)-f(x_0)}h.
$$

Since $x_0=1$, we obtain

$$
\frac{f(1+h)-f(1)}h.
$$

First, calculate each function value.

We know that

$$
f(1)=1^2=1.
$$

Also,

$$
f(1+h)=(1+h)^2.
$$

Expand the square:

$$
f(1+h)=1+2h+h^2.
$$

Substitute into the difference quotient:

$$
\frac{f(1+h)-f(1)}h=
\frac{1+2h+h^2-1}{h}.
$$

Simplify the numerator:

$$
=\frac{2h+h^2}{h}.
$$

Factor out $h$:

$$
=\frac{h(2+h)}{h}.
$$

For $h\neq0$, cancel the common factor:

$$
\boxed{\frac{f(1+h)-f(1)}h=2+h}
$$

### Step 4: Calculate the quotient for $h=1$

Substitute $h=1$:

$$
2+h=2+1.
$$

Therefore,

$$
\boxed{3}
$$

### Step 5: Calculate the quotient for $h=0.1$

Substitute $h=0.1$:

$$
2+h=2+0.1.
$$

Therefore,

$$
\boxed{2.1}
$$

### Step 6: Calculate the quotient for $h=0.01$

Substitute $h=0.01$:

$$
2+h=2+0.01.
$$

Therefore,

$$
\boxed{2.01}
$$

### Step 7: Compare the results

The exact derivative is

$$
f'(1)=2.
$$

The calculated difference quotients are:

| Value of $h$ | Difference quotient |
|---|---:|
| 1 | 3 |
| 0.1 | 2.1 |
| 0.01 | 2.01 |

As $h$ becomes smaller, the difference quotient approaches 2.

This agrees with the exact derivative.

### Step 8: Connect the calculations with the definition

The derivative is defined by the limit

$$
f'(1)=
\lim_{h\to0}
\frac{f(1+h)-f(1)}h.
$$

We already simplified the difference quotient to

$$
\frac{f(1+h)-f(1)}h=2+h.
$$

Therefore,

$$
f'(1)=\lim_{h\to0}(2+h).
$$

Evaluating the limit:

$$
f'(1)=2+0.
$$

Thus,

$$
\boxed{f'(1)=2}
$$

### Explanation

The numerical calculations show that the difference quotient approaches the derivative as $h$ approaches zero.

However, calculating only three values cannot prove that the limit exists.

A proof requires evaluating the limit mathematically, as shown above.

The numerical values provide an observation, while the limit calculation provides the mathematical justification.

## Final Answer

The chosen function is

$$
f(x)=x^2
$$

at the point

$$
x_0=1.
$$

The exact derivative is

$$
\boxed{f'(1)=2}
$$

The difference quotient is

$$
\boxed{2+h}
$$

Its values are:

$$
\boxed{
\begin{aligned}
h=1 &: \quad 3,\\
h=0.1 &: \quad 2.1,\\
h=0.01 &: \quad 2.01.
\end{aligned}
}
$$

Finally,

$$
\boxed{
\lim_{h\to0}\frac{f(1+h)-f(1)}h=2
}
$$
