Solution to last man standing
=============================

If we examine what happens when the number of people is a power of two, we
notice that the person who starts is also the last one to survive. For example,
with just two persons, it is clear that person number one is the sole survivor,
after killing number two.

With four persons, the first one kills number two. Number three kills number
four. After this, the sword has been passed a whole round back to person number
one. Now, only two persons remain (person number one and person number three).
We are now back to the previous situation with just two persons and the sword in
person number one's hands! Thus, it is not hard to see that when the number of
people is a power of two, the first one is always the last survivor (this can be
shown easily with [induction][1]).

Now, when the number of people `N` is different than a power of two, we need to
find the closest power of two smaller than `N`, i.e. `n = 2^floor(log2(N))`.
This is because after `N - n` deaths we have exactly `n` people left, i.e. a
power of two people. We already know from above that in this case, the first
person is the survivor. Thus, the person after `N - n` deaths will always be the
sole survivor!.

For instance, if `N = 100` we have `n = 64` and `N - n = 36`. The person holding
the sword after 36 deaths is person number `36 * 2 + 1 = 73` (since every other
person is killed). There are now 64 persons left (a power of two) and person
number 73 is holding the sword. You should therefore be person number 73 in
order to survive!

[1]: https://en.wikipedia.org/wiki/Mathematical_induction

[**Back to riddle**](../riddles/last.md)
