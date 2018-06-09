Prisoners and a light bulb
==========================

A prison guard is giving 100 prisoners a second chance for their death
sentences. The guard tells them that everyday, starting from tomorrow, he will
pick one prisoner randomly from his cell and bring him to his office. In the
office there is a light bulb wired to a power switch. The light bulb is
initially off and only has two states, on or off, triggered by the power
switch. While the prisoner is in the office, he has to do one of the following
things here: either _flip the power switch_ of the light bulb, and thus altering
its state (if it is off, this turns it on, and vice versa), or do
_nothing_. After the prisoner has chosen his action, he is brought back to his
cell and locked up. The process is then repeated the next day with another
random prisoner (it could be the same one, since the pick is random).

Now, if any prisoner, that is currently in the office, knows for certain that
every other prisoner has been in the office at least once, he can tell that to
the guard. If his claim is true, they are all spared, otherwise the game is over
and they all get killed!

The guard is a very patient man and has thus no time limit for his little
game. He will continue bringing a random prisoner to his office every day, until
some one dares to make the claim. His random pick is [uniformly
distributed](https://en.wikipedia.org/wiki/Uniform_distribution_(continuous)),
meaning that every prisoner has the _exact_ same probability to be picked
(1/100). Moreover, each one of the prisoners is contained in a different
isolated cell. There are no ways for them to communicate with each other at
all. They can also not leave any kind of "message" in the office for the others;
the guard only lets them flip the power switch for the bulb or do nothing.

The guard lets the prisoner discuss a strategy for a short period of time before
locking them in their respective cells for tomorrow's game. What is a winning
strategy for the prisoners, that spares them from their death sentences?

**[Solution](../solutions/bulb_solution.md)**
