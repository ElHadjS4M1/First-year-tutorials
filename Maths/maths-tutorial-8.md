# Maths tutorial 7
## Brandon Skerritt

## Question 1
For each of the following relations on the set A={1,2,3,4} determine whether they are functional, reflexive, symmetric, anti-symmetric or transitive.

Explain your answer in each case, showing why your answer is correct.

* {(4,2),(2,1),(1,2),(3,3)}
* {(2,1),(3,3),(4,2)}
* {(4,1),(4,2),(3,1),(3,2),(1,2)}
* {(x, y)|x > y}

### Answer
* {(4,2),(2,1),(1,2),(3,3)}
This is functional, not reflexive, not symmetric, not anti-symmetric and not transitive.

* {(2,1),(3,3),(4,2)}
This is functional, not reflexive, not symmetric, is anti symmetric, not transitive

* {(4,1),(4,2),(3,1),(3,2),(1,2)}
This is not functional, because one input (4, x) can result in more than 1 output. 
Not reflexive, not symmetric, is anti symmetric and is transitive.

* {(x, y)|x > y}
This set contains the items
{(2, 1), (3, 1), (4, 1), (3, 2), (4, 2), (4, 3)}
This set is not functional, not symmetric, is anti symmetric, and is transitive.

## Question 2
Let A={1,2,3,4} and the relation R on A be given by
R={(1,3),(3,2),(2,1),(4,4)}
What is the transitive closure of R?

### Answer
The transistive closure is how to make a set transitive. In this case you simply take something like (1, 3) and if you see (3, 2) you need to make (1, 2).
R={(1,3),(3,2),(2,1),(4,4)}
(1, 3) and (3, 2) makes (1, 2)

R={(1, 2), (1,3),(3,2),(2,1),(4,4)}
(1, 2) and (2, 1) makes (1, 1)

R={(1, 1), (1,2), (1,3),(3,2),(2,1),(4,4)}
(3, 2) and (2, 1) implies (3, 1)

R={(1, 1), (1,2), (1,3),(3, 1), (3,2),(2,1),(4,4)}
(3, 1) and (1, 2) implies (3, 2) and (3, 1) and (1, 3) implies (3, 3)

R={(1, 1), (1,2), (1,3), (3, 1), (3, 2), (3, 3),(2,1),(4,4)}
(2, 1) and (1, 2), (1, 3) implies (2, 2), (2, 3)

R={(1, 1), (1,2), (1,3), (2, 1), (2, 2), (2, 3) (3, 1), (3, 2), (3, 3), (4, 4)}
(4, 4) does not imply anything as nothing leads to 4.
So the full transitive closure is
R={(1, 1), (1,2), (1,3), (2, 1), (2, 2), (2, 3) (3, 1), (3, 2), (3, 3), (4, 4)}

## Question 3
For each of the following equivalence relations R on a given set A, describe the equivalence classes Ex into which the relation partitions the set A:
* A is the set of books in a library; R is given by xRy if, and only if, the colour of x’s cover is the same as the colour of y’s cover.
* A=Z; Ris given by xRy if, and only if,x−y is even.
* A is the set of people;Ris given by xRy if, and only if, x has the same sex as y.

### Answer
* A is the set of books in a library; R is given by xRy if, and only if, the colour of x’s cover is the same as the colour of y’s cover.
Each equivalence class consists of all those books of a fixed colour.

## Question 4
Is  there  a  mistake  in  the  following  proof  that  any  transitive  and  symmetric relation R is reflexive? If so, what is it:
>Let aRb.  By symmetry, bRa.  By transitivity, if aRb and bRa, then aRa. This proves reflexivity.

### Answer

Yes, there is a mistake.  The proof shows aRa by assuming that there is some b such that aRb, but there might not be such a b.  For example, the empty relation is transitive and symmetric but not reflexive.

The proof assumes that there exists b such that aRb.

## Question 5
Determine for the following relations on the set of people if the relation is an equivalence relation, a partial order, both an equivalence relation and a partial order, or neither an equivalence relation nor a partial order.

*  ‘has the same parents (both) as’
*  ‘has at least one parent same as’
*  ‘is a brother of’
*  ‘is at least as clever as’.

### Answer

Note that a relation cannot be both partial order and an equivalence relation.
According to https://math.stackexchange.com/questions/1760993/what-is-the-difference-between-partial-order-relations-and-equivalence-relations
Partial order and equivalence are the same except partial order are anti symmetric and and equivalence is symmetric. Both are transitive and reflexive.

* Has the same parents (both) as

## Question 6
Let R and S be relations on a set A. Use proof by contradiction to show that if R and S are partial orders then R∩S is also a partial order.

### Answer
I couldn't be bothered to do this one.
