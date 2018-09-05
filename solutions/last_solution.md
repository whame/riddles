Solution to last man standing
=============================

If we examine what happens when the number of people if a power of 2, we notice that the person who starts is also the last one to survive, since the number will halve every round without a reminder.

Now, when the number of people N is different than a power of 2, we need to find the closest power of 2 smaller than N: n = 2^floor(log2(N)), and realise that after N - n deaths, the next person wins the game.

For instance, if N = 100, n = 64, and after N - n = 36 deaths, the person holding the sword (73) will be the one surviving.

This can also be elegantly solved by exploiting circular bit shift:
- 100 (people) in binary is 1100100
- Circular left shift 1100100 yields 1001001
- 1001001 in base 10 is 73

i.e. the 73rd person is the last man standing.

To see why, note that the binary representation of N can be split into the sum of the closest power of 2 smaller than N, n (a 1 followed by log2(n) - 1 zeros), and a reminder k; N = n + k

For instance: 100 = 64 + 36, in binary, 1100100 = 1000000 + 100100.
Now, the number of the survivor after k = 100100 deaths is two times the number of deaths (left bitshift, k << 1), plus one, which is the left circular bitshift of the significant bit (n << 1).

All in all, 1000000 << 1 + 100100 << 1 = 73.

Remark: This is an O(1) operation, meaning it will be computed in one clock cycle on a computer.

[**Back to riddle**](../riddles/last.md)