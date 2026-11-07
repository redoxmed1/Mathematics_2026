### Exercise 14. Closest Point on a Line

**Problem**

Given a point $P=(4,1)$ and a line through the origin with direction $v=(1,2)$.

Using projection, find the closest point on the line, the distance from $P$ to the line, and verify that the appropriate vector is perpendicular to the direction of the line.

**Solution**

**1. Computing the projection**

The closest point on a line through the origin is the projection of $P$ onto the direction vector $v$.

The projection formula is:

$$
Q=\frac{P\cdot v}{v\cdot v}v
$$

First, calculate the dot product:

$$
P\cdot v=4(1)+1(2)
$$

$$
P\cdot v=6
$$

Next:

$$
v\cdot v=1^2+2^2
$$

$$
v\cdot v=5
$$

Substituting:

$$
Q=\frac65(1,2)
$$

Therefore:

$$
Q=\left(\frac65,\frac{12}{5}\right)
$$

This is the closest point on the line.

**2. Computing the distance from P to the line**

The vector from the closest point $Q$ to $P$ is:

$$
r=P-Q
$$

$$
r=(4,1)-\left(\frac65,\frac{12}{5}\right)
$$

$$
r=\left(\frac{20}{5}-\frac65,
\frac55-\frac{12}{5}\right)
$$

$$
r=\left(\frac{14}{5},-\frac75\right)
$$

The distance is the length of this vector.

$$
d=\|r\|
$$

$$
d=\sqrt{\left(\frac{14}{5}\right)^2+
\left(-\frac75\right)^2}
$$

$$
d=\sqrt{\frac{196}{25}+\frac{49}{25}}
$$

$$
d=\sqrt{\frac{245}{25}}
$$

$$
d=\frac{7\sqrt5}{5}
$$

**3. Verifying perpendicularity**

The shortest distance from a point to a line must be perpendicular to the line.

Therefore, we check:

$$
r\cdot v=0
$$

Substituting:

$$
r\cdot v=
\frac{14}{5}(1)+\left(-\frac75\right)(2)
$$

$$
=\frac{14}{5}-\frac{14}{5}
$$

$$
r\cdot v=0
$$

The perpendicularity condition is satisfied.

**4. Geometric interpretation**

The projection $Q$ is the closest point on the line to $P$.

The vector $r=P-Q$ connects the closest point to the original point.

Because this vector is perpendicular to the line, its length represents the minimum possible distance.

**Final Results**

$$
Q=\left(\frac65,\frac{12}{5}\right)
$$

$$
d=\frac{7\sqrt5}{5}
$$

$$
r\cdot v=0
$$
