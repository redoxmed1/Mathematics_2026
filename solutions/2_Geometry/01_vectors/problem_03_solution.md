### Exercise 3. Vector Normalization

**Problem**

For the vector

v = (3, 4)

1. Find a unit vector e with the same direction and orientation as v.
2. Check that the length of e is equal to 1.
3. Reconstruct v in the form v = ||v||e.
4. Explain what changes during normalization and what remains unchanged, paying particular attention to direction and orientation.

**Solution**

**Step 1. Calculate the length of v**

The length of a vector in R² is:

||v|| = √(x² + y²)

For v = (3, 4):

||v|| = √(3² + 4²)

||v|| = √(9 + 16)

||v|| = √25 = 5

**Step 2. Find the unit vector**

To normalize a vector, divide each component by its length:

e = v / ||v||

Therefore:

e = (3/5, 4/5)

**Step 3. Check that e is a unit vector**

Calculate its length:

||e|| = √((3/5)² + (4/5)²)

||e|| = √(9/25 + 16/25)

||e|| = √(25/25)

||e|| = 1

Therefore, e is a unit vector.

**Step 4. Reconstruct the original vector**

We must verify:

v = ||v||e

Substitute the values:

5(3/5, 4/5)

= (3, 4)

Therefore:

v = (3, 4)

The original vector has been reconstructed correctly.

**Step 5. Explain what changes and what remains unchanged**

During normalization:

- The length changes from 5 to 1.
- The direction remains unchanged.
- The orientation remains unchanged because the normalized vector points in the same direction as the original vector.

Normalization changes only the magnitude of the vector, not its direction or orientation.

**Final Answer**

The unit vector is:

e = (3/5, 4/5)

Its length is 1, and:

v = 5e = (3, 4)

The direction and orientation remain unchanged during normalization.
