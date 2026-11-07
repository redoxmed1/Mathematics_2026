### Exercise 6. Projection and Perpendicular Component

**Problem**

Find the projection of $u=(4,2)$ onto the direction $v=(1,1)$.

Then compute:

$$
r=u-\mathrm{proj}_v\,u
$$

and verify that $r\cdot v=0$. Explain this result geometrically.

**Solution**

**1. Computing the projection**

The projection formula is:

$$
\mathrm{proj}_v\,u=
\frac{u\cdot v}{v\cdot v}v
$$

First, calculate the dot product:

$$
u\cdot v=4(1)+2(1)=6
$$

Then calculate:

$$
v\cdot v=1^2+1^2=2
$$

Substituting into the projection formula:

$$
\mathrm{proj}_v\,u=
\frac{6}{2}(1,1)
$$

$$
\mathrm{proj}_v\,u=3(1,1)
$$

$$
\mathrm{proj}_v\,u=(3,3)
$$

**2. Computing the perpendicular component**

We use:

$$
r=u-\mathrm{proj}_v\,u
$$

Substituting the values:

$$
r=(4,2)-(3,3)
$$

$$
r=(1,-1)
$$

**3. Verifying perpendicularity**

Calculate the dot product:

$$
r\cdot v=1(1)+(-1)(1)
$$

$$
r\cdot v=1-1
$$

$$
r\cdot v=0
$$

Therefore, $r$ is perpendicular to $v$.

**4. Geometric interpretation**

The projection $(3,3)$ represents the component of $u$ parallel to the direction of $v$.

The vector $r=(1,-1)$ represents the remaining perpendicular component.

Together, they reconstruct the original vector:

$$
u=(3,3)+(1,-1)
$$

$$
u=(4,2)
$$

This shows that every vector can be decomposed into parallel and perpendicular components relative to a nonzero direction.

**Final Results**

$$
\mathrm{proj}_v\,u=(3,3)
$$

$$
r=(1,-1)
$$

$$
r\cdot v=0
$$
