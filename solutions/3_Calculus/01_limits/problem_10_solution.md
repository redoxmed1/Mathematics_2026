# Exercise 10: Continuity of a Piecewise Function

## Problem

Find the value of $a$ so that the following function is continuous at $x=2$:

$$
f(x)=\begin{cases}
ax+1, & x<2,\\
x^2-1, & x\geq2.
\end{cases}
$$

Explicitly compare the left-hand limit, right-hand limit, and function value.

## Solution

### Step 1: Recall the condition for continuity

A function is continuous at $x=2$ if the following three conditions are satisfied:

1. The left-hand limit exists.
2. The right-hand limit exists.
3. Both limits are equal to the function value at $x=2$.

In mathematical form:

$$
\lim_{x\to2^-}f(x)=
\lim_{x\to2^+}f(x)=
f(2).
$$

We calculate each quantity separately.

### Step 2: Calculate the left-hand limit

When $x<2$, the function is defined by

$$
f(x)=ax+1.
$$

Therefore,

$$
\lim_{x\to2^-}f(x)
=
\lim_{x\to2^-}(ax+1).
$$

Substituting $x=2$ gives

$$
\lim_{x\to2^-}f(x)
=
a(2)+1.
$$

Thus,

$$
\boxed{\lim_{x\to2^-}f(x)=2a+1}
$$

### Step 3: Calculate the right-hand limit

When $x\geq2$, the function is defined by

$$
f(x)=x^2-1.
$$

Therefore,

$$
\lim_{x\to2^+}f(x)
=
\lim_{x\to2^+}(x^2-1).
$$

Substituting $x=2$ gives

$$
\lim_{x\to2^+}f(x)
=
2^2-1.
$$

Simplifying:

$$
=4-1=3.
$$

Thus,

$$
\boxed{\lim_{x\to2^+}f(x)=3}
$$

### Step 4: Calculate the function value at $x=2$

We must use the correct branch of the piecewise function.

Since the second condition is $x\geq2$, the value at $x=2$ is calculated using

$$
f(x)=x^2-1.
$$

Therefore,

$$
f(2)=2^2-1.
$$

$$
f(2)=4-1.
$$

Thus,

$$
\boxed{f(2)=3}
$$

### Step 5: Find the value of $a$

For continuity, the left-hand limit must equal the right-hand limit and the function value.

We already calculated:

$$
\lim_{x\to2^-}f(x)=2a+1
$$

$$
\lim_{x\to2^+}f(x)=3
$$

$$
f(2)=3
$$

Therefore, we require

$$
2a+1=3.
$$

Subtract 1 from both sides:

$$
2a=3-1.
$$

$$
2a=2.
$$

Divide both sides by 2:

$$
a=\frac22.
$$

Therefore,

$$
\boxed{a=1}
$$

### Step 6: Verify continuity

We substitute $a=1$ into the left-hand limit:

$$
\lim_{x\to2^-}f(x)
=
2(1)+1
$$

$$
=2+1=3.
$$

The right-hand limit is

$$
\lim_{x\to2^+}f(x)=3.
$$

The function value is

$$
f(2)=3.
$$

Comparing the three results:

$$
\lim_{x\to2^-}f(x)
=
\lim_{x\to2^+}f(x)
=
f(2).
$$

Therefore,

$$
3=3=3.
$$

All three quantities are equal, so the function is continuous at $x=2$.

## Final Answer

The value of $a$ that makes the function continuous at $x=2$ is

$$
\boxed{a=1}
$$
