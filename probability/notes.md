Probability
===========

# Combinatorics

Combinatorics is just a fancy word for "counting", and it sounds a lot cooler.

## Permutations

In permutations, order matters.

The way I usually remember this is by thinking about how a "combination lock"
should really be called a "permutation lock".

Even though it is probably more common to want to count things where order does
*not* matter, instruction usually begins with permutations just because the
math is easier.

In permutations, since the order does not  matter, the equation is fairly
simple and intuitive. It looks something like this:

n! / (n - r)!

In other words, n * n-1 * n-2 all the way down to n-k.

## Combinations

In combinations, order does not matter so we have to divide out the duplicates.
This simply results in the addition of a term to the permutation equation.

n! / (n - k!)k!

Since k! is the number of ways that k can be taken from n, and we only care
about one way.

# Distributions

## Random Variables

A Random Variable, X, is an object that can be used to generate numbers in a
way that probabilistic statements about the generated numbers can be made.

The *variable* part is misleading here according to my previous understanding
as to what a variable is. However, after thinking about it a bit, it makes
sense. X is simply a variable with some constraints, namely it's distribution
and/or density function. It will take on any value within that distribution
according to the functions which define it.

It is different from a programming variable in the sense that it can take on
more than one value, or produce multiple values in the same program. However,
thinking about it from a functional programming perspective, the variable is
really just the function that defines the distribution of the ranndom variable.

## Distribution and Density functions



# Bayes theorem

# Independence
