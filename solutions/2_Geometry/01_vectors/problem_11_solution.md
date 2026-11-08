### Exercise 11. Decomposition into Parallel and Perpendicular Components

**Problem**

Decompose the vector

u = (3, 4)

into components parallel and perpendicular to

v = (1, 2).

1. Find the parallel component u_parallel using projection.
2. Find the perpendicular component u_perpendicular.
3. Perform both requested checks:

   - Verify that u = u_parallel + u_perpendicular.
   - Verify that u_perpendicular · v = 0.

4. Explain why these are two independent checks of correctness.

**Solution**

**Step 1. Calculate the parallel component**

The projection formula is:

u_parallel = (u · v / v · v)v

First, calculate the dot product:

u · v = (3)(1) + (4)(2)

u · v = 3 + 8 = 11

Now calculate:

v · v = (1)(1) + (2)(2)

v · v = 1 + 4 = 5

Substitute into the projection formula:

u_parallel = (11/5)(1, 2)

Therefore:

u_parallel = (11/5, 22/5)

**Step 2. Calculate the perpendicular component**

The perpendicular component is the difference between the original vector and its parallel component:

u_perpendicular = u - u_parallel

Substitute:

u_perpendicular = (3, 4) - (11/5, 22/5)

Write the coordinates with a common denominator:

u_perpendicular = (15/5 - 11/5, 20/5 - 22/5)

Therefore:

u_perpendicular = (4/5, -2/5)

**Step 3. First check: reconstruct the original vector**

We must verify:

u = u_parallel + u_perpendicular

Substitute:

(11/5, 22/5) + (4/5, -2/5)

Add the components:

= (15/5, 20/5)

= (3, 4)

Therefore:

u_parallel + u_perpendicular = u

The first check is correct.

**Step 4. Second check: verify perpendicularity**

We must verify:

u_perpendicular · v = 0

Substitute:

(4/5, -2/5) · (1, 2)

Calculate:

= (4/5)(1) + (-2/5)(2)

= 4/5 - 4/5

= 0

Therefore, the perpendicular component is orthogonal to v.

**Step 5. Explain why the checks are independent**

The first check verifies that the two components reconstruct the original vector correctly.

The second check verifies that the perpendicular component is actually perpendicular to the direction of v.

These checks test two different properties:

- Reconstruction: the components add up to the original vector.
- Orthogonality: the perpendicular component has a zero dot product with v.

Both conditions are necessary to confirm the decomposition.

**Final Answer**

Parallel component:

u_parallel = (11/5, 22/5)

Perpendicular component:

u_perpendicular = (4/5, -2/5)

First check:

u_parallel + u_perpendicular = (3, 4) = u

Second check:

u_perpendicular · v = 0

Both checks are satisfied.
