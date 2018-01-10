# Maths Tutorial 7
## Brandon Skerritt

## Question 1
Let A = {1,2,3} and B = {a, b}. Determine the set A×B

### Answer

All elements of A times by the first element of B then second etc.
First step: 1a, 2a
Second step: 2a, 2b
Third step: 3a, 3b

AxB = {1a, 2a, 2a, 2b, 3a, 3b}

## Question 2
Let A be a set. Determine the set A×∅

### Answer
∅ is the empty set. Therefore anything times the empty set is also the empty set.
Answer: ∅.

## Question 3
Which ordered pairs are in the relation R={(x, y)|x > y} on the set A={1,2,3,4}?

### Answer
So a relation on itself (A X A) is every single possible combination in that set. But in this instance we want every single pair where x is more than y. Therefore this is:

R = {(2,1 ), (3, 1), (3, 2), (4, 1), (4, 2), (4, 3)}

## Question 4
List all the binary relations on the set {0,1}.

### Answer
So a binary relation is just any relation that contains every element in the relation. In this instance the binary relation is just:
{(0, 1), (1, 0)}
As there are only 2 possible ways to change the set of {0, 1} into an order due to 2 items being in the set.

## Question 5
List the set of ordered pairs and draw the graphical representation of the relation R between {1,2,3,4} and {a, b, c} with the matrix:


```
T   F   F
F   F   T
F   T   F
T   F   F
```

### Answer
So to do this we first need to decide what is T and what is F. We draw this

```
     a   b   c
1    T   F   F
2    F   F   T
3    F   T   F
4    T   F   F
```

And this is what the relationship looks like. Now we simply list what is T (True).
Relation = {(1, a), (2, c), (4, a)}

## Question 6
Let R be the relation on {1,2,3,4} given by xRy if, and only if, x−y=0. Represent R in the following ways:
* As a set of ordered pairs
* In graphical form
* In matrix form

### Answer
Okay so this question is a bit awkward. the relation rule is x - y = 0, so the first one take away the second must must equal 0. Because of this, x and y has to be equal because it'll only ever be <0 or >0 if it isn't equal. Therefore the set of ordered pairs is:
R = {(1, 1), (2, 2), (3, 3), (4, 4)}

In graphical form this would be a diagraph.

As a matrix this would be:

```
    1 2 3 4
1   T F F F
2   F T F F
3   F F T F
4   F F F T
```

## Question 7
Consider the following family tree:

![Family tree](https://screenshotscdn.firefoxusercontent.com/images/e5822296-f336-4db5-94cd-ab2c2ea1f80e.png)

Let A={Thelma, Thaddeus, Karen, Peter, Meg} be the set of all family members and B={Thaddeus, Peter} be the set of male members.

Let R be the relation between the sets A and B consisting of pairs(a, b), where a is a parent of b. Let S be the relation between sets B and A consisting of pairs(a, b), where a and 5b are siblings (brothers or sisters).

* Represent relations R and S in the matrix form.
* Use the matrix forms to compute R◦S and S◦R

### Answer
R = {(Themla, Thaddeus), (Thelma, Karen), (Thelma, Peter), (Peter, Meg)}
S = {(Thadeus, Karen), (Thadeus, Peter), (Karen, Peter)}

R in matrix form:
```
            Thelma Peter
Thaddeus    T       F
Karen       T       F
Peter       T       F
Meg         F       T
```
