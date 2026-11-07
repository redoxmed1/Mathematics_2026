### Exercise 15. Complete Classification of a Line Relative to a Plane

**Problem**

Let

$$
L:p+tv,\qquad \Pi:n\cdot x=d.
$$

State the conditions distinguishing the three cases: one intersection point, parallel with no common points, and the line contained in the plane. Then illustrate each case with your own simple numerical example.

**Solution**

**1. Understanding the general equations**

The line is:

$$
L:p+tv
$$

where:

- $p$ is a point on the line.
- $v$ is the direction vector of the line.
- $t$ is a real parameter.

The plane is:

$$
\Pi:n\cdot x=d
$$

where:

- $n$ is the normal vector of the plane.
- $d$ is a constant.

To determine the relative position of the line and plane, substitute the line equation into the plane equation.

$$
n\cdot(p+tv)=d
$$

Using the distributive property:

$$
n\cdot p+t(n\cdot v)=d
$$

The value of $n\cdot v$ determines the relationship between the line and plane.

**2. Case 1: One intersection point**

If:

$$
n\cdot v\neq0
$$

The line is not parallel to the plane.

There is exactly one intersection point.

The parameter is obtained from:

$$
t=\frac{d-n\cdot p}{n\cdot v}
$$

**Numerical example**

Consider the plane:

$$
\Pi:z=0
$$

Its normal vector is:

$$
n=(0,0,1)
$$

Choose the line:

$$
L=(0,0,1)+t(1,0,-1)
$$

The direction vector is:

$$
v=(1,0,-1)
$$

Calculate:

$$
n\cdot v=0(1)+0(0)+1(-1)
$$

$$
n\cdot v=-1\neq0
$$

Therefore, the line intersects the plane at one point.

To find the intersection:

$$
z=1-t=0
$$

$$
t=1
$$

Substituting:

$$
(x,y,z)=(1,0,0)
$$

The intersection point is:

$$
I=(1,0,0)
$$

**3. Case 2: Parallel with no common points**

If:

$$
n\cdot v=0
$$

and:

$$
n\cdot p\neq d
$$

The line is parallel to the plane but does not lie in it.

Therefore, there are no intersection points.

**Numerical example**

Consider again the plane:

$$
\Pi:z=0
$$

Choose the line:

$$
L=(0,0,1)+t(1,2,0)
$$

The direction vector is:

$$
v=(1,2,0)
$$

Calculate:

$$
n\cdot v=0(1)+0(2)+1(0)
$$

$$
n\cdot v=0
$$

Now check the starting point:

$$
p=(0,0,1)
$$

$$
n\cdot p=0(0)+0(0)+1(1)
$$

$$
n\cdot p=1
$$

Since:

$$
1\neq0
$$

The line is parallel to the plane and has no common points with it.

**4. Case 3: The line is contained in the plane**

If:

$$
n\cdot v=0
$$

and:

$$
n\cdot p=d
$$

The direction vector is parallel to the plane and the starting point belongs to the plane.

Therefore, the entire line lies in the plane.

**Numerical example**

Consider the plane:

$$
\Pi:z=0
$$

Choose the line:

$$
L=(0,0,0)+t(1,2,0)
$$

The direction vector is:

$$
v=(1,2,0)
$$

Calculate:

$$
n\cdot v=0(1)+0(2)+1(0)
$$

$$
n\cdot v=0
$$

Check the starting point:

$$
p=(0,0,0)
$$

$$
n\cdot p=0
$$

Since:

$$
n\cdot p=d=0
$$

The entire line lies in the plane.

**5. General classification**

The three possible cases can be summarized as follows.

**Case 1: One intersection point**

$$
n\cdot v\neq0
$$

**Case 2: Parallel with no common points**

$$
n\cdot v=0
$$

$$
n\cdot p\neq d
$$

**Case 3: The line is contained in the plane**

$$
n\cdot v=0
$$

$$
n\cdot p=d
$$

**Final Conclusion**

The relative position of a line and a plane can be determined using only two dot products.

The first dot product, $n\cdot v$, determines whether the line crosses the plane or is parallel to it.

The second condition, $n\cdot p=d$, distinguishes between a parallel line outside the plane and a line completely contained in the plane.
