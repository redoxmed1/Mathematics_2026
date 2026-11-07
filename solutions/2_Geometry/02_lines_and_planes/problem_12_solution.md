### Exercise 12. Intersection Line of Two Planes

**Problem**

Find a parametric equation of the line that is the intersection of

$$
x+y+z=3,\qquad x-y+z=1.
$$

Find its direction vector in two ways: from the system of equations and from the cross product of the normal vectors. Compare the results.

**Solution**

**1. Identifying the normal vectors**

The first plane is:

$$
\Pi_1:x+y+z=3
$$

Its normal vector is:

$$
n_1=(1,1,1)
$$

The second plane is:

$$
\Pi_2:x-y+z=1
$$

Its normal vector is:

$$
n_2=(1,-1,1)
$$

**2. Finding the intersection line from the system**

We solve the two equations simultaneously:

$$
\begin{cases}
x+y+z=3, \\
x-y+z=1.
\end{cases}
$$

Subtract the second equation from the first:

$$
2y=2
$$

Therefore:

$$
y=1
$$

Substitute into the first equation:

$$
x+1+z=3
$$

$$
x+z=2
$$

Choose $x=t$ as the free parameter.

Then:

$$
z=2-t
$$

The parametric equations are:

$$
\begin{cases}
x=t, \\
y=1, \\
z=2-t.
\end{cases}
$$

Therefore, the intersection line is:

$$
L=(0,1,2)+t(1,0,-1)
$$

Its direction vector is:

$$
v=(1,0,-1)
$$

**3. Finding the direction vector using the cross product**

The direction of the intersection line must be perpendicular to both normal vectors.

Therefore:

$$
v=n_1\times n_2
$$

$$
v=
\begin{pmatrix}
1(1)-1(-1) \\
1(1)-1(1) \\
1(-1)-1(1)
\end{pmatrix}
$$

$$
v=(2,0,-2)
$$

This vector can be simplified by dividing by $2$:

$$
v=(1,0,-1)
$$

**4. Comparing the results**

From the system of equations:

$$
v_1=(1,0,-1)
$$

From the cross product:

$$
v_2=(2,0,-2)
$$

These vectors are scalar multiples:

$$
v_2=2v_1
$$

Therefore, they represent the same direction.

Both methods give the same intersection line.

**Final Result**

Parametric equation:

$$
L=(0,1,2)+t(1,0,-1)
$$

Direction vector:

$$
v=(1,0,-1)
$$
