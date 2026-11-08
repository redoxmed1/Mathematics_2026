### Exercise 15. Comparing Directions Using the Cosine of the Angle

**Problem**

Given:

$$
a=(1,2,1)
$$

$$
b=(2,4,2)
$$

$$
c=(2,0,3)
$$

For each pair, compute:

$$
\frac{u\cdot v}{\|u\|\,\|v\|}
$$

Order the pairs by increasing angle between the vectors. Explain why for $a$ and $b$ the value is $1$ even though the vectors have different lengths.

**Solution**

**1. Computing the lengths**

For vector $a$:

$$
\|a\|=\sqrt{1^2+2^2+1^2}
$$

$$
\|a\|=\sqrt6
$$

For vector $b$:

$$
\|b\|=\sqrt{2^2+4^2+2^2}
$$

$$
\|b\|=\sqrt{24}
$$

For vector $c$:

$$
\|c\|=\sqrt{2^2+0^2+3^2}
$$

$$
\|c\|=\sqrt{13}
$$

**2. Computing the cosine for the pair (a,b)**

First, calculate the dot product:

$$
a\cdot b=1(2)+2(4)+1(2)
$$

$$
a\cdot b=12
$$

Using the cosine formula:

$$
\cos\theta_{ab}=
\frac{a\cdot b}{\|a\|\|b\|}
$$

$$
=\frac{12}{\sqrt6\sqrt{24}}
$$

Since:

$$
\sqrt6\sqrt{24}=12
$$

Therefore:

$$
\cos\theta_{ab}=1
$$

The angle is:

$$
\theta_{ab}=0^\circ
$$

**3. Computing the cosine for the pair (a,c)**

First, calculate the dot product:

$$
a\cdot c=1(2)+2(0)+1(3)
$$

$$
a\cdot c=5
$$

Using the cosine formula:

$$
\cos\theta_{ac}=
\frac{5}{\sqrt6\sqrt{13}}
$$

$$
\cos\theta_{ac}=\frac{5}{\sqrt{78}}
$$

Approximately:

$$
\cos\theta_{ac}\approx0.566
$$

Therefore:

$$
\theta_{ac}\approx55.52^\circ
$$

**4. Computing the cosine for the pair (b,c)**

First, calculate the dot product:

$$
b\cdot c=2(2)+4(0)+2(3)
$$

$$
b\cdot c=10
$$

Using the cosine formula:

$$
\cos\theta_{bc}=
\frac{10}{\sqrt{24}\sqrt{13}}
$$

Since:

$$
\sqrt{24}\sqrt{13}=2\sqrt{78}
$$

We obtain:

$$
\cos\theta_{bc}=\frac{5}{\sqrt{78}}
$$

Approximately:

$$
\cos\theta_{bc}\approx0.566
$$

Therefore:

$$
\theta_{bc}\approx55.52^\circ
$$

**5. Ordering the pairs by increasing angle**

The calculated angles are:

$$
\theta_{ab}=0^\circ
$$

$$
\theta_{ac}\approx55.52^\circ
$$

$$
\theta_{bc}\approx55.52^\circ
$$

Therefore, the order is:

$$
(a,b)<(a,c)=(b,c)
$$

**6. Geometric explanation**

The vectors $a$ and $b$ have different lengths, but they point in exactly the same direction.

This is because:

$$
b=2a
$$

The cosine of the angle between two vectors depends on their directions, not their individual lengths.

Since the angle between $a$ and $b$ is zero degrees:

$$
\cos(0^\circ)=1
$$

Therefore, the cosine value is $1$ even though the vectors have different lengths.

**Final Results**

$$
\cos\theta_{ab}=1
$$

$$
\cos\theta_{ac}=\frac{5}{\sqrt{78}}
$$

$$
\cos\theta_{bc}=\frac{5}{\sqrt{78}}
$$

The increasing order of angles is:

$$
(a,b)<(a,c)=(b,c)
$$
