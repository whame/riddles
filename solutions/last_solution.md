Solution to last man standing
=============================

The simple solution is to simply cross of every second person around a
circle of 100 points until only one is left.

You could also realize that in the first round, all people with even
numbers die. Following this idea, you can find patterns for the
following rounds. However, this will take nine cumbersome rounds to
complete.

This can all be elegantly solved by exploiting circular bit shift:
- 100 (people) in binary is 1100100
- Circular left shift 1100100 yields 1001001
- 1001001 in base 10 is 73

i.e. the 73rd person is the last man standing, and this is the
position you would want to choose in order to survise.

Remark: This is an O(1) operation, meaning it will be computed in one
clock cycle on a computer.

[**Back to riddle**](../riddles/last.md)