Solution to sphere and tetrahedron
==================================

This solution to this problem is preferably started out with a
divide-and-conquer approach, i.e. "Randomly select 3 points on the surface of a
circle. Construct an inscribed triangle containing the random points as
vertices."

Now, consider the first two points, p1 and p2, have been selected. By bisecting
the circle with each of these points, the circle now consists of four quadrants,
though they may not be of the same size. p3 must now be inside the quadrant that
is opposite to p1 and p2. So what is the probability of the third point being in
that quadrant?

Look at the problem the other way around: Choose two lines bisecting the
circle. You do not yet know on which ends of these lines p1 and p2 are. Now
randomly choose p3. This point is now in one of the quadrants. The two lines can
only be constructed with p1 and p2 in 4 different ways, equally probable, out of
which only one way results in p3 being in the correct quadrant. Hence, the
probability of the triangle containing the center of the circle is 1/4.

Similarly, for a sphere the probability is one octant, i.e. 1/8.

Remark: Now you have the solution for two and three dimensions. What about *n*
dimensions?

[**Back to riddle**](../riddles/sphere.md)

