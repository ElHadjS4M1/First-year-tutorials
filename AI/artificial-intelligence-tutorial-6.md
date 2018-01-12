# Artifical Intelligence tutorial 5
## Brandon Skerritt

## Question 1
Which of the following are true?  Check using truth tables or defining relevant interpretations directly.
* {p1,(p1⇒p2),(p2⇒p3)}|=p3
* {(p1⇒p2)}|= (p2⇒p1)
* {(p1∨¬p2)}|=p1
* {(p1∧¬p1)}|=p2

### Answers
{p1,(p1⇒p2),(p2⇒p3)}|=p3
The turnstile |= symbol means entailment. A |= B is only true if A is true.
And "," means and.

p1 | p2 | p3 | p1 => p2 | p2 => p3
--- | --- |  --- | --- | ---
1 | 1 | 1 | 1 | 1
1 | 1 | 0 | 1 | 0
1 | 0 | 0 | 0 | 0
1 | 0 | 1 | 0 | 1
0 | 1 | 1 | 1 | 1
0 | 1 | 0 | 1 | 1
0 | 0 | 1 | 1 | 1
0 | 0 | 0 | 1 | 1

It follows that for every interpretation I, if
I(p1) = 1, I(p1 ⇒ p2) = 1, I(p2 ⇒ p3) = 1,
then I(p3) = 1
Because the left handside is true, then the right hand side is true.

{(p1⇒p2)}|= (p2⇒p1)

p1 | p2 | p1=>p2 | p2 => p1
--- | --- | --- | ---
1 | 1 | 1 | 1
1 | 0 | 0 | 1
0 | 1 | 1 | 0
0 | 0 | 1 | 1

This is not true. Take I such that I(p1) = 0 and I(p2) = 1. Then I(p1 ⇒ p2) = 1 but I(p2 ⇒ p1) = 0.
Therefore the right hand side is not always true when the left hand side is true, breaking the rule of the turnstile |= symbol.

{(p1∨¬p2)}|=p1

p1 | p2 | ~p2 | p1 V ~p2 
--- | --- | --- | ---
1 | 1 | 0 | 1
1 | 0 | 1 | 1
0 | 1 | 0 | 0
0 | 0 | 1 | 1

This is not true because everytime the right hand side is not true when p1 is not true (last one).

{(p1∧¬p1)}|=p2

p1 | p2 | ~p1 | p1 v ~p1
--- | --- | --- | ---
1 | 1 | 0 | 1
1 | 0 | 0 | 0
0 | 1 | 1 | 1
0 | 0 | 1 | 0

Not true

## Question 2
What is the probability that a randomly selected integer chosen uniformly from the first 100 positive integers is odd? To answer the question, first define the probability space (S, P).

### Answer

The problem space is the 100 numbers and the chance of selecting an odd number from the problem space is 50 / 100 = 1/2.

## Question 3
Suppose that I have four fair coins with values 1p, 2p, 5p and 10p. I call the 1p coin and the 2p coin “low-value” coins and the other twocoins “high-value coins”.

### Question 3 part a
What is the probability that, when I flip the coins, the 1p and the 5p come up heads, and the other two coins come up tails? To answer the question, first define the probability space (S, P).

So the problem space is every possible change of the coins coming up either heads or tails. There are 4 coins and each coin has a chance of being {H, T} so therefore the problem becomes 2^4 which is 16.

Another way to look at it is like this:
There are 4 coins
```
0 0 0 0 
```
And each coin has a 1/2 chance of either being heads or tails
```
{H, T} {H, T} {H, T} {H, T}
```
Now one problem outcome could be
```
H H T T
```
And another could be
```
H T H H
```
So there is 2 outcomes for every possible coin and combinations matter. So we could simply do 4 * 4 (using the counting rule from combinatorics) because we have a set of 4 coins and each 4 coin could be something. Another way to view this is to literally count the counts yourself.
```
H H H H
H H H T
H H T H
H T H H
T H H H
T T H H
T H T H
T H H T
H H T T
H T T T
T T T H
T T T T
....
```
But this will take too long.
It's better to consider that there are 2 options, heads or tails, and there are 4 coins. So 2^4 is 16.

Since each outcome is equally likely, each coin has a 1/16 chance of being heads or tails.

What is the probability that, when I flip the coins, the 1p and the 5p come up heads, and the other two coins come up tails? To answer the question, first define the probability space (S, P).

Okay so this is one instance of an event of 4 coins being flipped. So there is a 1/2 chance of each coin either being heads or tails and there are 4 coins so 1/2 ^ 4 is 16. Another way of looking at this is that there are 2 outcomes for each coin, heads and tails, so it becomes 2^4. Either way its ^4 because there are 4 coins and the number that it is powering is the probability.

## Question 3 part b
What is the probability that at least one of the low-value coins comes up tails?

### Answer

So we have 4 coins, 2 high value, 2 low value.

High High Low Low
and we want to work out the chance that a low value coin comes up tails.

So there are 2 low value coins and each one has a 1/2 chance of coming up tails

So with the last one we want to work out the probability of one of the low value coins coming up tails.

To do this we can take 1 - (probability of getting a low value coin)
The probability of getting a low value coin is either 1/16 for
X X X T
another 1/16 for
X X T X
Another 1/16 for
X X T T
So that's
1 - (1/16 * 3)

No wait this is wrong!

So an event is where all the coin flips *matter*
So it wouldn't be 
X X T X
it would be 
H T T H
which is different to
H H T H
even though they both have the same answer (what we previously thought)
So because we want either one of the coins to be tails, there are more than 3 possible events because the first two coins are also included in the event
so it *ISN'T* 1 - (1/16 * 3) and is much more than *3 !
So therefore the easiest way to do this is to work out the probability of both coins landing on tails seperately
So that is
P(A) + P(B) 
But we want to work out the union of these two events, whats the union of the 2 probabilities that *either* one lands on tails
both events are disjoint (they dont effect each other) so therefore the union of 2 disjoint events is defined as 
P(E1∪E2) = P(E1) + P(E2) - P(E1∩E2)
Because we include the chance of getting tails on both of them twice (venn diagram)
So this becomes
P(1/2) + P(1/2) - P(1/4) = 3/4
P(E1∩E2) = P(E1) * P(E2)

## Question 3 part c
What is the probability that at least three of the coins come uptails?

### Answer

So this event exists like so
H T T T
or 
H T T T 
But we could easily just add together the probability of each getting a tails
This is the union of 5 disjoint events. The union of 4 different coins coming up tails and the union that all the coins come up tails. So the union of 4 selected coins (any coins) coming up tails with the union of all coins coming up tails.
So the probability of each of these events is 1/16 (probability of the event happening we calculated previously) and since there are 5 events that is 5 * 1/16 which is 5/16.

## Question 4
What probability should be assigned to the outcome of heads when a biased coin is tossed,  if heads is three times as likely to come up as tails?  What probability should be assigned to the outcome of tails?
The P of tails is P(3/4) and the probability of heads is P(1/4).


