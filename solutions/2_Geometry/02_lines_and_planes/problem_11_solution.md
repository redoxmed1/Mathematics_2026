### Exercise 11. Plane Containing a Line and a Point

**Problem**

Find the equation of the plane containing

$$
(x,y,z)=(1,0,2)+t(1,1,-1)
$$

and the point $P=(0,2,1)$. Check that both the entire line and the point lie in the plane you obtain.

**Solution**

**1. Identifying the point and direction vector**

From the line equation:

$$
p=(1,0,2)
$$

$$
v=(1,1,-1)
$$

The additional point is:

$$
P=(0,2,1)
$$

**2. Constructing a second direction vector**

We construct a vector from the point on the line to the additional point.

$$
w=P-p
$$

$$
w=(0-1,2-0,1-2)
$$

$$
w=(-1,2,-1)
$$

We now have two direction vectors lying in the plane:

$$
v=(1,1,-1)
$$

$$
w=(-1,2,-1)
$$

**3. Finding the normal vector**

The normal vector is obtained from the cross product:

$$
n=v\times w
$$

$$
n=
\begin{pmatrix}
1(-1)-(-1)(2) \\
(-1)(-1)-1(-1) \\
1(2)-1(-1)
\end{pmatrix}
$$

$$
n=(1,2,3)
$$

**4. Finding the plane equation**

The plane passes through:

$$
p=(1,0,2)
$$

Using the normal vector:

$$
n=(1,2,3)
$$

The equation is:

$$
1(x-1)+2(y-0)+3(z-2)=0
$$

Simplifying:

$$
x-1+2y+3z-6=0
$$

$$
x+2y+3z-7=0
$$

**5. Checking the entire line**

The line is:

$$
\begin{cases}
x=1+t, \\
y=t, \\
z=2-t.
\end{cases}
$$

Substitute into the plane equation:

$$
(1+t)+2t+3(2-t)-7=0
$$

$$
1+t+2t+6-3t-7=0
$$

$$
0=0
$$

The equation is satisfied for every value of $t$.

Therefore, the entire line lies in the plane.

**6. Checking the additional point**

Substitute $P=(0,2,1)$:

$$
0+2(2)+3(1)-7=0
$$

$$
0+4+3-7=0
$$

$$
0=0
$$

The additional point also belongs to the plane.

**Final Result**

The plane equation is:

$$
x+2y+3z-7=0
$$

Normal vector:

$$
n=(1,2,3)
$$
