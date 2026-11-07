### Exercise 10. Projection of a Point onto a Plane

**Problem**

Find the orthogonal projection of $P=(2,1,3)$ onto the plane $x+y+z=3$, and then find the reflection of $P$ across this plane. Check that the midpoint of the segment joining the point and its reflection lies on the plane.

**Solution**

**1. Identifying the normal vector**

The plane is:

$$
x+y+z=3
$$

Its normal vector is:

$$
n=(1,1,1)
$$

The point is:

$$
P=(2,1,3)
$$

**2. Computing the projection**

The orthogonal projection is found using:

$$
Q=P-\frac{n\cdot P-d}{n\cdot n}n
$$

where $d=3$.

First, calculate:

$$
n\cdot P=1(2)+1(1)+1(3)
$$

$$
n\cdot P=6
$$

Next:

$$
n\cdot n=1^2+1^2+1^2=3
$$

Substituting:

$$
Q=P-\frac{6-3}{3}(1,1,1)
$$

$$
Q=(2,1,3)-(1,1,1)
$$

Therefore:

$$
Q=(1,0,2)
$$

**3. Checking the projection**

Substitute $Q$ into the plane equation:

$$
1+0+2=3
$$

The projection belongs to the plane.

**4. Computing the reflection**

The projection is the midpoint between the original point and its reflection.

Therefore:

$$
R=2Q-P
$$

Substituting:

$$
R=2(1,0,2)-(2,1,3)
$$

$$
R=(2,0,4)-(2,1,3)
$$

$$
R=(0,-1,1)
$$

**5. Checking the midpoint**

The midpoint of $P$ and $R$ is:

$$
M=\frac{P+R}{2}
$$

$$
M=\frac{(2,1,3)+(0,-1,1)}{2}
$$

$$
M=\frac{(2,0,4)}{2}
$$

$$
M=(1,0,2)
$$

This is exactly the projection $Q$.

Now check the plane equation:

$$
1+0+2=3
$$

The midpoint belongs to the plane.

**6. Geometric interpretation**

The projection is the closest point on the plane to the original point.

The reflection lies on the opposite side of the plane at the same distance.

The plane passes through the midpoint of the segment connecting the original point and its reflection.

**Final Results**

Orthogonal projection:

$$
Q=(1,0,2)
$$

Reflection:

$$
R=(0,-1,1)
$$

Midpoint:

$$
M=(1,0,2)
$$
