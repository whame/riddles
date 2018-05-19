Solution to greedy pirates
==========================

Yet another divide-and-conquer problem. Consider the chip consisting of:

* 2 pirates - The captain will propose he gets all the coins and then vote for
  himself, thus getting 50% of the votes and all the coins.

* 3 pirates - The captain will propose the lowest ranked pirate gets 1 coin and
  he then keeps the rest. Rationale: If he proposes anything that will end up in
  the other two pirates voting nay, he will die, and the next pirate in rank
  will get all coins according to the example with two pirates. This means that
  the lowest ranked pirate will get no coins, ergo, the lowest ranked pirate
  knows that getting just 1 coin from the captain is a better deal than if the
  captain walks the plank and the next pirate takes all for himself.

* 4 pirates - In the example with 3 pirates, the captain gets 2/3 votes. By now
  proposing the second lowest ranked pirate gets 1 coin, the same rationale holds
  and the captain gets 50% of the votes.

* 5 pirates - Again, using the same rationale: If pirate 1 is the captain, then
  offering pirates 3 and 5 one coin will grant him 3/5 votes.

* 6 pirates - Offer pirates 4 and 2 one coin grants him 3/6 votes.

In general, this works with *n* pirates where the captain proposes that pirates
1+2k gets one coin, where k=1,2,3,...

[**Back to riddle**](../solutions/pirates.md)