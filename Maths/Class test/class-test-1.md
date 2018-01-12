# Maths class test 1
## Brandon Skerritt

## Question 1
Suppose that U={1,2,3,4,5,6,7}is the universal set, A={x∈N|2< x <7}, B={3,7}, and C={3,4,5,6}.

## Question 1 a
List the elements of the set B∪(A∩C)

A = 3, 4, 5, 6

### Answer
(A∩C) =  3, 4, 5, 6
B∪(A∩C) = {3, 4, 5, 6, 7}

## Question 1 b
What is the characteristic vector of (A∆B)∩C?

### Answer
A∆B = {4, 5, 6, 7}

(A∆B)∩C = {4, 5, 6}

## Question 2
Which of the following statements are true?

* {a, b, c}⊆{b, c, a}−{b}

So {b, c, a}−{b} is just {c, a}.
Thus the question is
is the set containing {a, b, c} a subset of the set containing {c, a}?
Well no, because the first set contains {b} and the second set doesn't.

* {a}⊆{a, b}
The set containing the element of "a" is indeed a subset of {a, b}.

* {b, c}⊆{c, b}
Yes, b, c is a subset of c, b.
The first set contains all the elements in the second set, and order doesn't matter. Thus it is a subset.

* {a, b, c}∆{b}={a, c}
{a, b, c}∆{b}
is all elements that are in set on the left and set on the right but not in both. Since the element b is in both it is removed.
{a, c}.
Thus the question becomes
{a, c} = {a, c}
Which is true for obvious reasons.

## Question 3
Which of the following statements are true

* x∈{x}
Is the singular element x an element of the set containing the element x? Yes.

* {x}⊆{x}
Is the set containing the element x a subset of the set containing the element x? They are the same, so yes it is a subset.

* {x}∈{x}
Is the set containing the element x an element of the set containing the element x? Nope. If it was, it would be like this {x}∈{{x}}.

* {x}∈{{x}}
Yes, this is correct. See above.

* ∅⊆{x}
Yes, the empty set is always a subset of *any* set.

* ∅∈{x}
No, the empty set is not an element of the set containing _only_ x.

## Question 4
Which of the following are true for every negative integer x and every negative integer y?

So both integers are negative and they are integers (whole numbers).

* x−y is a positive integer
This isn't *always* true. Let's try an example. -2 - -1 is -1, which is still negative.

* x×y is a natural number.
Let's try an example. -2 * -2 is -4. Natural numbers are positive whole numbers, so this isn't true either. This is wrong! Any negative times a negative is a positive.

* x+y is a negative integer
-6 + -3 = -9. If x and y are negative integers then this is true.

* x/y is a rational.
This is true because -6 / -8 is true.

* y/x is a rational
This is still true.

## Question 5
How many prime numbers are odd?

### Answer
All of them apart from the number 2.

## Question 6
Let A={1,3,5} and B={x, y, z}. Define f:A→B by specifying that
>(1) = y, f(3) = z, f(5) = y
Determine whether f is injective, surjective or bijective (remember, it can have more than one property).

### Answer
Okay so injectivty is where not all answers have an output. This is not injective because all items in A have at least 1 output in B.
Surjectivty is where B can have more than 1 A. This is surjective because y can be reached from f(5) and f(1).
This isn't bijective because bijectity is where it is both injective and surjective.

## Question 7
Let f:R→R be the function defined byf(x) = 2*x+1.  Determine whether f is injective,surjective or bijective.

### Answer
To check for injectivity you simply just do this
2\*x1+1 = 2\*x2+1
2\*x1 = 2\*x2
x1 = x2
Therefore it is injective

To check for surjectivity you just have to think about it (alot)
So the function isn't surjective because 1 output can't be reached from 2 different inputs. If you have x = 2 so 2*2 = 4 + 1 = 5, now try to find a way to get 5 again. The closet thing we could do is -2 but -2 * 2 = -4 + 1 = -3, which isn't 5. Try again with 1. 2 * 1 = 2 + 1 = 3. 2 * -1 = -2 + 1 = -1. It's impossible to get the same output from 2 different inputs, so this isn't surjective.

Because it's not surjective, it's also not bijective.

## Question 8
Let X={1,2,3},Y={a, b, c, d, e}and Z={x, y, z}.  Define functions f:X→Y and g:Y→Zby specifying that:
> f(1) = b, f(2) = a, f(3) = c
and
> g(a) =  x, g(b) =y, g(c) = y, g(d) = z, g(e) = z.
Determine g◦f. What is the range of g◦f?

### Answer
so if you have pen and paper it's best to do this as a diagraph, but we'll try without.
So GoF is defined as
>g(f(1)) = y
>g(f(2)) = x
>g(f(3)) = y
So we take the output from f(1) etc and then given the output b we put this into g.

The range of GoF is all the possible outputs which is {y, x, y} but because set theory doesn't allow repition it's {x, y}.

## Question 9
Let X={1,2},Y={a, b, c} and Z={x, y, z}. Let f:X→Y and g:Y→Z be such that:
> g(a) =x, g(b) =y, g(c) =x
And
> g◦f(1) =x, g◦f(2) =x.

Determine F.

### Answers

So GoF(1) = x. So we simply return it. like so
So when 1 is input into F, it transform it into X. So therefore f(1) = a
So when 2 is input into F, it transform into X. So therefore f(2) = c.

## Question 10
How many people do you need to have in a room in order to guarantee that at least two of them have a birthday on the same day of the week?

### Answer
So a person can be born on 1 of 7 days (monday tuesday wednesday etc...) and once you have 8 people in a room, two of them have to be born on the same day. So the answer is 8.

## Question 11
How many integers from 100 through 999 must you pick in order to be sure that at least two of them have a digit in common? (For example,256 and 530 have the common digit 5.)

### Answer
So this is a simple counting problem.
There are 10 integers that it could be and 3 spaces
> X X X
Any one of those X's could be one of 10 integers
And you want at least 2 of them to have the same digit in common.
So 10 digits and they can be put over any of the numbers
Well, if you pick 2 random numbers there isn't a very high chance of getting 2 digits in common.






