# Exercise 14: A 0/0 Limit with Trigonometry

## Problem

Compute

$$
\lim_{x\to0}\frac{1-\cos x}{x^2}.
$$

Justify the result without using l'Hôpital's rule, using a trigonometric identity and the fundamental limit.

## Solution

Let

$$
L=\lim_{x\to0}\frac{1-\cos x}{x^2}.
$$

We use the trigonometric identity

$$
1-\cos x=2\sin^2\left(\frac{x}{2}\right).
$$

Substitute this identity into the limit:

$$
L=
\lim_{x\to0}
\frac{2\sin^2\left(\frac{x}{2}\right)}{x^2}.
$$

Rewrite the denominator using

$$
x^2=4\left(\frac{x}{2}\right)^2.
$$

Therefore,

$$
L=
\lim_{x\to0}
\frac{2\sin^2\left(\frac{x}{2}\right)}
{4\left(\frac{x}{2}\right)^2}.
$$

Simplifying:

$$
L=
\frac12
\lim_{x\to0}
\frac{\sin^2\left(\frac{x}{2}\right)}
{\left(\frac{x}{2}\right)^2}.
$$

We can write this as

$$
L=
\frac12
\lim_{x\to0}
\left(
\frac{\sin\left(\frac{x}{2}\right)}
{\frac{x}{2}}
\right)^2.
$$

Using the fundamental trigonometric limit,

$$
\lim_{u\to0}\frac{\sin u}{u}=1,
$$

where

$$
u=\frac{x}{2},
$$

we obtain

$$
L=\frac12\cdot1^2.
$$

Therefore,

$$
\boxed{L=\frac12}
$$

## Explanation

We used the identity

$$
1-\cos x=2\sin^2\left(\frac{x}{2}\right)
$$

to transform the original expression into one involving the fundamental trigonometric limit.

This proves the result without using l'Hôpital's rule.

## Final Answer

$$
\boxed{\frac12}
$$
