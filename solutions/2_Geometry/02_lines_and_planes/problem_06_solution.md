### Exercise 6. Angle Between Planes

**Problem**

Given

$$
\Pi_1:x+y+z=1,\qquad \Pi_2:x-y=2.
$$

First use the normal vectors to decide whether the planes are parallel. If not, compute the angle between them and explain why the normal vectors alone are enough for this calculation.

**Solution**

**1. Identifying the normal vectors**

The normal vector is obtained from the coefficients of the plane equation.

For the first plane:

$$
\Pi_1:x+y+z=1
$$

Its normal vector is:

$$
n_1=(1,1,1)
$$

For the second plane:

$$
\Pi_2:x-y=2
$$

Its normal vector is:

$$
n_2=(1,-1,0)
$$

**2. Checking whether the planes are parallel**

Two planes are parallel if their normal vectors are scalar multiples of each other.

Since:

$$
n_1=(1,1,1)
$$

$$
n_2=(1,-1,0)
$$

The vectors are not scalar multiples.

Therefore, the planes are not parallel.

**3. Computing the angle between the planes**

The angle between two planes is the acute angle between their normal vectors.

We use the formula:

$$
\cos\theta=
\frac{|n_1\cdot n_2|}
{\|n_1\|\|n_2\|}
$$

First, calculate the dot product:

$$
n_1\cdot n_2=1(1)+1(-1)+1(0)
$$

$$
n_1\cdot n_2=0
$$

Calculate the lengths:

$$
\|n_1\|=\sqrt{1^2+1^2+1^2}
$$

$$
\|n_1\|=\sqrt3
$$

$$
\|n_2\|=\sqrt{1^2+(-1)^2+0^2}
$$

$$
\|n_2\|=\sqrt2
$$

Substitute:

$$
\cos\theta=\frac{0}{\sqrt3\sqrt2}
$$

$$
\cos\theta=0
$$

Therefore:

$$
\theta=90^\circ
$$

**4. Geometric interpretation**

The normal vectors are perpendicular because their dot product is zero.

Since the angle between the normal vectors is $90^\circ$, the planes are perpendicular.

The normal vectors are sufficient because they completely determine the orientation of the planes.

**Final Results**

$$
n_1=(1,1,1)
$$

$$
n_2=(1,-1,0)
$$

$$
\theta=90^\circ
$$

The planes are perpendicular and not parallel.
