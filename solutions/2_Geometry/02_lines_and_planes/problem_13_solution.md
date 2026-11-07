### Exercise 13. Closest Point on a Plane

**Problem**

Find the point on the plane $x+2y+2z=4$ closest to $P=(3,0,0)$. Give the distance and check that the segment joining the two points is perpendicular to the plane.

**Solution**

**1. Identifying the normal vector**

The plane is:

$$
x+2y+2z=4
$$

Its normal vector is:

$$
n=(1,2,2)
$$

The given point is:

$$
P=(3,0,0)
$$

**2. Computing the closest point**

The closest point is the orthogonal projection of $P$ onto the plane.

We use:

$$
Q=P-\frac{n\cdot P-d}{n\cdot n}n
$$

where $d=4$.

First, calculate:

$$
n\cdot P=1(3)+2(0)+2(0)
$$

$$
n\cdot P=3
$$

Next:

$$
n\cdot n=1^2+2^2+2^2
$$

$$
n\cdot n=9
$$

Substituting:

$$
Q=P-\frac{3-4}{9}(1,2,2)
$$

$$
Q=P+\frac19(1,2,2)
$$

Therefore:

$$
Q=
\left(
3+\frac19,
\frac29,
\frac29
\right)
$$

$$
Q=\left(\frac{28}{9},\frac29,\frac29\right)
$$

**3. Checking that Q belongs to the plane**

Substitute the coordinates:

$$
\frac{28}{9}
+2\left(\frac29\right)
+2\left(\frac29\right)=4
$$

$$
\frac{28}{9}+\frac49+\frac49=4
$$

$$
\frac{36}{9}=4
$$

$$
4=4
$$

The point belongs to the plane.

**4. Computing the distance**

The distance between $P$ and $Q$ is:

$$
d(P,Q)=\|P-Q\|
$$

The distance formula from a point to a plane gives:

$$
d=
\frac{|n\cdot P-4|}{\|n\|}
$$

Substituting:

$$
d=\frac{|3-4|}{\sqrt{1^2+2^2+2^2}}
$$

$$
d=\frac1{\sqrt9}
$$

$$
d=\frac13
$$

**5. Checking perpendicularity**

Calculate the vector joining $P$ to $Q$:

$$
Q-P=
\left(
\frac{28}{9}-3,
\frac29,
\frac29
\right)
$$

$$
Q-P=
\left(\frac19,\frac29,\frac29\right)
$$

This vector is a scalar multiple of the normal vector:

$$
Q-P=\frac19(1,2,2)
$$

Therefore, the segment joining $P$ and $Q$ is perpendicular to the plane.

**Final Results**

Closest point:

$$
Q=\left(\frac{28}{9},\frac29,\frac29\right)
$$

Distance:

$$
d=\frac13
$$
