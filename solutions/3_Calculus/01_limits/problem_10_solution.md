
## Exercise 10 — Continuity of a Piecewise Function

```markdown
# Exercise 10: Continuity of a Piecewise Function

## Problem

Find $a$ so that

$$
f(x)=
\begin{cases}
ax+1,&x<2,\\
x^2-1,&x\geq2
\end{cases}
$$

is continuous at $x=2$.

Explicitly compare the left-hand limit, right-hand limit, and function value.

## Solution

A function is continuous at $x=2$ if

$$
\lim_{x\to2}f(x)=f(2).
$$

This requires the left-hand limit, right-hand limit, and function value to be equal.

### Part 1: Left-Hand Limit

For $x<2$, the function is

$$
f(x)=ax+1.
$$

Therefore,

$$
\lim_{x\to2^-}f(x)
=
\lim_{x\to2^-}(ax+1).
$$

Substitute $x=2$:

$$
\boxed{\lim_{x\to2^-}f(x)=2a+1}
$$

### Part 2: Right-Hand Limit

For $x\geq2$, the function is

$$
f(x)=x^2-1.
$$

Therefore,

$$
\lim_{x\to2^+}f(x)
=
\lim_{x\to2^+}(x^2-1).
$$

Substitute $x=2$:

$$
\lim_{x\to2^+}f(x)=2^2-1.
$$

$$
\boxed{\lim_{x\to2^+}f(x)=3}
$$

### Part 3: Function Value

Since $2\geq2$, we use the second part of the piecewise definition:

$$
f(2)=2^2-1.
$$

Therefore,

$$
\boxed{f(2)=3}
$$

### Part 4: Find the Value of a

For continuity, the left-hand limit must equal the right-hand limit and the function value.

Thus,

$$
2a+1=3.
$$

Subtract 1 from both sides:

$$
2a=2.
$$

Divide both sides by 2:

$$
\boxed{a=1}
$$

### Part 5: Verification

Substitute $a=1$ into the left-hand expression:

$$
\lim_{x\to2^-}f(x)=2(1)+1=3.
$$

The right-hand limit is

$$
\lim_{x\to2^+}f(x)=3.
$$

The function value is

$$
f(2)=3.
$$

Therefore,

$$
\lim_{x\to2^-}f(x)
=
\lim_{x\to2^+}f(x)
=
f(2)=3.
$$

The function is continuous at $x=2$.

## Final Answer

$$
\boxed{a=1}
$$
