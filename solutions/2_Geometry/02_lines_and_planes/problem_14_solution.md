### Exercise 14. Contrast: Intersection and Parallelism

**Problem**

From the point $P=(0,0,1)$, two lines are drawn with direction vectors

$$
v_1=(2,1,-1),\qquad v_2=(2,1,0).
$$

For each line, analyze its position relative to the plane $z=0$.

For the line that intersects the plane, find the intersection point. For the other line, explain how you can recognize parallelism without solving an equation.

**Solution**

**1. Identifying the normal vector**

The plane is:

$$
z=0
$$

Its normal vector is:

$$
n=(0,0,1)
$$

Both lines start at:

$$
P=(0,0,1)
$$

**2. Analyzing the first line**

The first direction vector is:

$$
v_1=(2,1,-1)
$$

Calculate its dot product with the normal vector:

$$
v_1\cdot n=2(0)+1(0)+(-1)(1)
$$

$$
v_1\cdot n=-1
$$

Since the dot product is not zero, the line is not parallel to the plane.

Therefore, it intersects the plane at exactly one point.

**3. Finding the intersection point of the first line**

The parametric equation is:

$$
L_1=(0,0,1)+t(2,1,-1)
$$

Therefore:

$$
\begin{cases}
x=2t, \\
y=t, \\
z=1-t.
\end{cases}
$$

To find the intersection, use the plane equation:

$$
z=0
$$

Substitute:

$$
1-t=0
$$

$$
t=1
$$

Now calculate the coordinates:

$$
x=2(1)=2
$$

$$
y=1
$$

$$
z=0
$$

Therefore, the intersection point is:

$$
I_1=(2,1,0)
$$

**4. Analyzing the second line**

The second direction vector is:

$$
v_2=(2,1,0)
$$

Calculate its dot product with the normal vector:

$$
v_2\cdot n=2(0)+1(0)+0(1)
$$

$$
v_2\cdot n=0
$$

Therefore, the second line is parallel to the plane or contained in it.

However, its starting point is:

$$
P=(0,0,1)
$$

Substituting into the plane equation:

$$
z=1\neq0
$$

The starting point does not belong to the plane.

Therefore, the second line is parallel to the plane and has no intersection with it.

**5. Geometric comparison**

The first line has a direction vector that is not perpendicular to the plane's normal vector. Therefore, it crosses the plane.

The second line has a direction vector perpendicular to the plane's normal vector. Since its starting point is outside the plane, it never intersects it.

**Final Results**

First line:

$$
v_1\cdot n=-1
$$

It intersects the plane at:

$$
I_1=(2,1,0)
$$

Second line:

$$
v_2\cdot n=0
$$

It is parallel to the plane and has no common points with it.
