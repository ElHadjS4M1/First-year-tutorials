# Artificial Intelligence Tutorial 7
## Brandon Skerritt

## Question 1
We first continue Question 3 from Exercise 6.  Recall that we have four fair coins with values 1p, 2p, 5p and 10p.  We call the 1p coin and the 2p coin “low-value” coins and the other two coins “high-value coins”.Assume we flip the coins.

### Question 1 part a
What is the probability that at least three of the coins come uptails,  conditioned on the fact that at least one of the low-value coins comes up tails?

### Answer
So the probability of one of the low value coins coming up tails is 3/4

So the probability of getting 3 coins being tails is the probability of P(Tails | Probability of a low value coin coming up tails)
So P(Tails | 3/4) = P(a union b) / 3/4
So P(Tails | 3/4) = P(5/16) / 3/4 = 5/12


### Question 1 part b
Is the event that at least three of the coins come up tails indepen-dent of the event that at least one of the low-value coins comesup tails?
P(F|G) = 5/12 and P(F) = 5/16. Becuase there are not the same they are not independent.

## Question 2
Let ( S,P ) be a probability space and let A and A 1 ,...,A n be events in S such that
* Ai∩Aj=∅for all 1≤i < j≤n;
* A1∪···∪An=S

I don't think this question is important for the exam so I skipped over it.

## Question 3
Suppose you are a witness to a nighttime hit-and-run accident involving a taxi in Madrid.  All taxis in Madrid are blue or green.  Assume that  9  out  of  10  taxis  are  green.   You  swear,  under  oath,  that  the taxi was blue.  Extensive testing shows that,  under the dim lighting conditions, discrimination between blue and green is 75% reliable. Compute  the  most  likely  colour  of  the  taxi.   In  your  computation,distinguish carefully between the event that the taxi is blue and the event that it appears blue.
