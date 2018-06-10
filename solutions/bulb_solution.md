Solution to prisoners and a light bulb
======================================

One prisoner is assigned as a _counter_. The role of this counter is to keep
track of how many prisoners that have entered the office. The counter thus has
to count 99 other prisoners before he can tell the guard.

Now, when one of the other 99 prisoners enters the office and the light bulb is
on, he does nothing. If it is off, he turns it on but and only if he has not
done this before. When the counter enters the room and sees the bulb on, he
switches it off and increments his count with one. Since prisoners only switches
the light bulb on if they have not done this before, the switched on light bulb
encountered by the counter is a different unique prisoner. Thus, after the
counter has switched the light bulb off 99 times he can now tell the guard that
every prisoner has entered the office.

**Remark**: This solution, for 100 prisoners, has an expected run time of
10417.74 days (28.54 years). There are more complex and efficient
solutions. However, the question of optimality is still open. For more details
please see this
[paper](https://www.ocf.berkeley.edu/~wwu/papers/100prisonersLightBulb.pdf).

[**Back to riddle**](../riddles/bulb.md)