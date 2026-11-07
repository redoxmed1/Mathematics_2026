### Exercise 4. Plane Through Three Points

**Problem**

Find the equation of the plane through

$$
A=(1,0,0),\quad B=(0,1,0),\quad C=(0,0,1).
$$

First construct two vectors lying in the plane, and then use the cross product. Check the resulting equation on all three points.

**Solution**

**1. Constructing two vectors in the plane**

The first vector is:

$$
\overrightarrow{AB}=B-A
$$

$$
\overrightarrow{AB}=(0-1,1-0,0-0)
$$

$$
\overrightarrow{AB}=(-1,1,0)
$$

The second vector is:

$$
\overrightarrow{AC}=C-A
$$

$$
\overrightarrow{AC}=(0-1,0-0,1-0)
$$

$$
\overrightarrow{AC}=(-1,0,1)
$$

**2. Finding the normal vector using the cross product**

The cross product produces a vector perpendicular to both vectors.

$$
n=\overrightarrow{AB}\times\overrightarrow{AC}
$$

$$
n=
\begin{pmatrix}
1(1)-0(0) \\
0(-1)-(-1)(1) \\
(-1)(0)-1(-1)
\end{pmatrix}
$$

$$
n=(1,1,1)
$$

Therefore, the normal vector is:

$$
n=(1,1,1)
$$

**3. Finding the plane equation**

The general equation is:

$$
x+y+z+d=0
$$

Substitute point $A=(1,0,0)$:

$$
1+0+0+d=0
$$

$$
d=-1
$$

Therefore, the plane equation is:

$$
x+y+z-1=0
$$

**4. Checking all three points**

For point $A=(1,0,0)$:

$$
1+0+0-1=0
$$

For point $B=(0,1,0)$:

$$
0+1+0-1=0
$$

For point $C=(0,0,1)$:

$$
0+0+1-1=0
$$

All three points satisfy the equation.

**Final Results**

$$
\overrightarrow{AB}=(-1,1,0)
$$

$$
\overrightarrow{AC}=(-1,0,1)
$$

$$
n=(1,1,1)
$$

Plane equation:

$$
x+y+z=1
$$
