# Exercise 9: One-Sided Limits and an Asymptote

## Problem

Analyze the left-hand and right-hand limits of

$$
f(x)=\frac1{x-2}
$$

as $x\to2$.

Does the two-sided limit exist? Interpret the result on a sketch of the graph and identify the vertical asymptote.

## Solution

We study the function

$$
f(x)=\frac1{x-2}.
$$

The denominator becomes zero at $x=2$, so the function is undefined at this point.

### Part 1: Left-Hand Limit

We calculate

$$
\lim_{x\to2^-}\frac1{x-2}.
$$

When $x$ approaches 2 from the left, $x$ is smaller than 2.

Therefore,

$$
x-2<0.
$$

The denominator approaches zero through negative values.

Consequently, the fraction becomes increasingly negative:

$$
\boxed{\lim_{x\to2^-}\frac1{x-2}=-\infty}
$$

### Part 2: Right-Hand Limit

Now calculate

$$
\lim_{x\to2^+}\frac1{x-2}.
$$

When $x$ approaches 2 from the right, $x$ is greater than 2.

Therefore,

$$
x-2>0.
$$

The denominator approaches zero through positive values.

Consequently, the fraction becomes increasingly positive:

$$
\boxed{\lim_{x\to2^+}\frac1{x-2}=+\infty}
$$

### Part 3: Two-Sided Limit

For a two-sided limit to exist as a finite real number, the left-hand and right-hand limits must agree.

Here,

$$
\lim_{x\to2^-}f(x)=-\infty
$$

while

$$
\lim_{x\to2^+}f(x)=+\infty.
$$

Therefore, the two-sided limit does not exist.

$$
\boxed{\lim_{x\to2}\frac1{x-2}\text{ does not exist}}
$$

### Part 4: Vertical Asymptote and Sketch

The denominator becomes zero at $x=2$, and the function grows without bound near this value.

Therefore, the graph has a vertical asymptote:

$$
\boxed{x=2}
$$

A qualitative sketch is:

```text
             y
             |
             |             /
             |            /
             |           /
-------------|----------|---------- x
             |          2
             |          |
          \  |          |
           \ |          |
            \|          |
