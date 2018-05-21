Solution to Devil's chessboard
==============================

The coins have binary values (two possible values, heads and
tails). Conveniently, the number of squares on a chessboard can be perfectly
represented in binary as there are 64, or 2^6, squares. In other words, any
square on the board can be represented using six bits, naming the squares 0-63.

Now we need to figure out how to use the six bits. Make six groups, each
corresponding to specific region of the chessboard:

Group 1: Rows 1, 3, 5, 7

Group 2: Rows 1, 2, 5, 6

Group 3: Rows 1, 2, 3, 4

Group 4: Columns 1, 3, 5, 7

Group 5: Columns 1, 2, 5, 6

Group 6: Columns 1, 2, 3, 4

Now, count all the heads in each group. If the number is odd, the value is a 1,
if the number is even, the value is 0.

Example: If there are odd number of heads in groups 1, 5 and 6 but even number
of heads in groups 2, 3 and 4, then the resulting binary value is 100011.

Now let's say that "the magic square" is number 27, i.e. 011011.

By XOR operation of these two binary numbers, we get the square of the coin that
we need to flip in order to represent "the magic square", e.g:

100011
011011
------
111000

111000 = 56

If you flip coin 56 in this case, then when your friend comes in and examines
the groups for their parity, he will read get the binary number 011011 which is
27, "the magic square".


[**Back to riddle**](../riddles/chess.md)