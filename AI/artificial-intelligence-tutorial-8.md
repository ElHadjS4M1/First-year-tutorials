# Artificial Intelligence Tutorial 8
## Brandon Skerritt

## Question 1
Let BuysBeer be a random variable with values 0 and 1 for false and true,  respectively,  and let CustomerType be a random variable with values single,couple, and family.  The joint probability distribution for BuysBeer and CustomerType is given by
![stuff](https://screenshotscdn.firefoxusercontent.com/images/a740c708-3105-457e-8acd-812caa68f338.png)
Compute the following probabilities:
* P(BuysBeer= 1)
* P(CustomerType = couple)
* P(CustomerType=couple,BuysBeer= 1)
* P(CustomerType=couple|BuysBeer= 1)

### Answers
* P(BuysBeer= 1)
0.26
* P(CustomerType = couple)
0.46
* P(CustomerType=couple,BuysBeer= 1)
0.14
* P(CustomerType=couple|BuysBeer= 1)
| here simply means divided. so 0.14 divided by 0.26. 0.14/0.26.

## Question 2
Based  on  the  populations  60776228,  5116900  and  2980700  of  England (E), Scotland (S), and Wales (W), the prior probability that a randomly  selected  person  from  these  countries  is  living  in  England,Scotland, or Wales is approximately 0.88, 0.08, and 0.04, respectively.Consider the random variableCountrywith valuesE,S, andWandthe probability distribution given by

> P(Country) = (0.88,0.08,0.04)

Consider  the  random  variable Mothertongue that  takes  values Eng,Scot, and Welsh.  Consider the following fictitious conditional probabilities:
* P(Mothertongue=Eng|Country=E) = 0.95;
* P(Mothertongue=Eng|Country=S) = 0.7;
* P(Mothertongue=Eng|Country=W) = 0.6
* P(Mothertongue=Scot|Country=E) = 0.04;
* P(Mothertongue=Scot|Country=S) = 0.3;
* P(Mothertongue=Scot|Country=W) = 0.0;
* P(Mothertongue=Welsh|Country=E) = 0.01;
* P(Mothertongue=Welsh|Country=S) = 0.0;
* P(Mothertongue=Welsh|Country=W) = 0.4

Compute:

* The joint probability distribution P(Country, Mothertongue).
* The marginal distribution P(Mothertongue).

### Answers
* The joint probability distribution P(Country, Mothertongue).
the Comma "," means and.
So this is asking for probability distribution of P(country and mothertongue)
or p(country ^ mothertongue)
We can use the product rule which we already know
P(a|b) = p(a and b) / p(b)
With simple algebraic manipulation we get
p(a and b) = p(a|b) . p(b)
Therefore 

> p(Country and Mothertongue) = P(country | Mothertongue) P(mothertongue)

So this is asking for the probability distribution of country and mothertongue.


There are 3 mothertongues, Welsh, Scot, Eng. There are 3 countries: E S W
Thus

_ | Country = E | Country = S | Country = W
--- | --- | --- | ---
Mothertongue = Welsh | 0.01 | 0 | 0.4
Mothertongue = Scot | 0.04 | 0.3 | 0
Mothertongue = Eng | 0.95 | 0.7 | 0.6

So this is just a table for all the mothertongues / countries. Now we want to work out
P(country = E | Mothertongue = Eng) * P(mothertongue = Eng)
for every one of these.
