### Exercise 13. Do Four Points Lie in One Plane?

**Problem**

Given the four points:

A = (0, 0, 0)

B = (1, 2, 0)

C = (0, 1, 1)

D = (2, 5, 1)

1. Construct the vectors AB and AC using the coordinates of the points.
2. Find the normal vector n = AB × AC.
3. Construct the vector AD.
4. Calculate the dot product AD · n and determine whether it is equal to zero.
5. Decide whether D lies in the plane determined by A, B and C.
6. Explain why AD · n = 0 is the coplanarity criterion.

**Solution**

**Step 1. Construct vector AB**

Subtract the coordinates of A from the coordinates of B:

AB = B - A

AB = (1 - 0, 2 - 0, 0 - 0)

Therefore:

AB = (1, 2, 0)

**Step 2. Construct vector AC**

AC = C - A

AC = (0 - 0, 1 - 0, 1 - 0)

Therefore:

AC = (0, 1, 1)

**Step 3. Find the normal vector**

The cross product of AB and AC gives a vector perpendicular to both.

n = AB × AC

n =

| i    j    k |
| 1    2    0 |
| 0    1    1 |

Calculate each component:

First component:

2(1) - 0(1) = 2

Second component:

0(0) - 1(1) = -1

Third component:

1(1) - 2(0) = 1

Therefore:

n = (2, -1, 1)

This is a normal vector to the plane determined by A, B and C.

**Step 4. Construct vector AD**

AD = D - A

AD = (2 - 0, 5 - 0, 1 - 0)

Therefore:

AD = (2, 5, 1)

**Step 5. Calculate the dot product**

We must check:

AD · n = 0

Substitute:

(2, 5, 1) · (2, -1, 1)

Calculate:

= (2)(2) + (5)(-1) + (1)(1)

= 4 - 5 + 1

= 0

Therefore:

AD · n = 0

**Step 6. Explain the coplanarity criterion**

The vectors AB and AC lie in the plane determined by A, B and C.

Their cross product n is perpendicular to this plane.

The vector AD connects point A to point D.

If AD · n = 0, then AD is perpendicular to the normal vector n.

This means AD lies in the plane determined by AB and AC.

Therefore, point D also belongs to that plane.

The condition AD · n = 0 is the coplanarity criterion because it checks whether the fourth point lies in the same plane as the first three points.

**Final Answer**

AB = (1, 2, 0)

AC = (0, 1, 1)

Normal vector:

n = (2, -1, 1)

AD = (2, 5, 1)

Dot product:

AD · n = 0

Therefore, the four points A, B, C and D are coplanar.
