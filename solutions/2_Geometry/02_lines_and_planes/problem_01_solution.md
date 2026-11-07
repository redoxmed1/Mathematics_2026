### Exercise 1. Line Through Two Points

**Problem**

Find the equation of the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation you obtain.

**Solution**

**1. Finding the direction vector**

The direction vector is obtained by subtracting the coordinates of point $A$ from point $B$.

$$
\overrightarrow{AB}=B-A
$$

$$
\overrightarrow{AB}=(4-1,-1-2)
$$

$$
\overrightarrow{AB}=(3,-3)
$$

Therefore, a direction vector is:

$$
v=(3,-3)
$$

**2. Finding the parametric equation**

The parametric equation of a line is:

$$
(x,y)=A+tv
$$

Substituting the point and direction vector:

$$
(x,y)=(1,2)+t(3,-3)
$$

Separating the coordinates:

$$
\begin{cases}
x=1+3t, \\
y=2-3t.
\end{cases}
$$

**3. Finding a normal vector**

A normal vector must be perpendicular to the direction vector.

We can choose:

$$
n=(1,1)
$$

Checking:

$$
n\cdot v=1(3)+1(-3)=0
$$

Therefore, $n=(1,1)$ is a valid normal vector.

**4. Finding the general equation**

The general equation of a line is:

$$
ax+by+c=0
$$

Using the normal vector $(1,1)$ and point $A=(1,2)$:

$$
1(x-1)+1(y-2)=0
$$

Simplifying:

$$
x-1+y-2=0
$$

$$
x+y-3=0
$$

**5. Checking both points**

For point $A=(1,2)$:

$$
1+2-3=0
$$

For point $B=(4,-1)$:

$$
4+(-1)-3=0
$$

Both points satisfy the equation.

**Final Results**

Direction vector:

$$
v=(3,-3)
$$

Normal vector:

$$
n=(1,1)
$$

Parametric equation:

$$
\begin{cases}
x=1+3t, \\
y=2-3t.
\end{cases}
$$

General equation:

$$
x+y-3=0
$$
