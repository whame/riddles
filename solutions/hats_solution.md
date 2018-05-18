Solution to prisoners with hats
==============================

Clearly, the first prisoner can not know his hat color in any way. He thus has a
50 % chance of guessing his hat color correctly. However, he can see all other
prisoners hats. He either sees an odd number or an even number of white hats in
front of him. If he sees an odd number of hats, he says "black", otherwise
"white".

Suppose the first one says "black", meaning he can see an odd number of white
hats in front of him. The second prisoner in the line hears this, and can
determine his own color by counting how many white hats he can see in front of
him. Suppose he sees an odd number of white hats. Since the first prisoner said
"black", then he must have a black hat. This is because he also sees an odd
number of white hats in front of him and can thus not have a white hat himself
(otherwise the first prisoner would instead have seen an even number of white
hats and answered "white"). Similarly, suppose the second prisoner instead sees
an even number of white hats. Since the first prisoner said "black", he must
then now have a white hat (otherwise the first prisoner would also have seen an
even number of white hats and answered "white").

On the other hand, suppose the first one instead says "white", meaning he can
see an even number of white hats in front of him. The second prisoner can
however now again, by counting how many white hats he can see, determine his own
color with the same reasoning as before. Indeed, all of the other prisoners
adopt exactly the same reasoning. By just keeping track of the previous
prisoners answers and counting how many white hats they can see, they can
determine their own hat color. Thus, with this strategy you can save all but the
first prisoner.

In general, this strategy works for _n_ prisoners, saving _n_-1 prisoners. This
is also optimal, since we save all prisoners except the first one, who can not
be saved definitely.
