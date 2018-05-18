Hypersphere and n-simplex tetrahedron
=====================================

This solution to this problem is preferably started out with a
divide-and-conquer approach.

Consider the 2-dimensional equivalent of the problem, i.e. randomly choosing
three points on the surface of a circle and finding the probability of the
triangle, formed by these three points, containing the center of the circle.

First randomly choose two points and from each these points bisect the circle,
thus creating four quadrants. In order for the third point to form a triangle
containing the center, it must lie in the quadrant formed by the bisecttions
from the former two points. Even though the quadrants may not be equisized, the
two bisectors could only be created by four constillations of two points. Hence,
the probability of the formed triangle to contain the center of the sphere is
1/4.

Similarly, for a sphere the probability is one octant, 1/8, or better yet,
2^-3^.

Through mathematical induction, it can be shown that this holds for any
dimension, i.e. resulting in a probability of 2^-n^.

