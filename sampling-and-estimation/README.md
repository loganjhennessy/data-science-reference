# Statistical Modeling

A statistical model is the *set of all candidate distributions (or, random
variables), one of which we suspect generated our data.*

The trick here is that the statistical model is actually a bunch of possible
distributions. It, in and of itself, does not do much for us other than
enumerate possibilities.

What we want to do is figure out *which* of the models actually generated our
data, for this we have the following methods:

  - Eyeball Method
  - Method of Moments
  - Maximum Likelihood Method

Remember also that *parameter* in this context refers to a statistical
parameter such as *mean*, *median*, or *mode*.

## Eyeball Method

There isn't too much to say here. You draw a bunch of candidate distributions
against your data and eyeball which one is closest.

This has obvious drawbacks, but may suffice in very simple situations.

## Method of Moments

For more rigorous distribution selection, we can use the Method of Moments.

The process is fairly straightforward:

  1. Find the function that represents the population expectation, mu
  2. Find the *sample mean* (i.e. sample expectation) of your data
  3. Equate your sample mean to the function for population expectation

## [Maximum Likelihood Estimation](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation)

Rather than using the sample parameters to estimate the population parameters,
The MLE method seeks to find the parameters that represent the distribution
from which the data has a maximum likelihood of coming from.

## Random Variables

A random variable, X, is an object that can be used to generate numbers, in a
way that valid probabilistic statements about the generated numbers can be made.

## Kolmogorov-Smirnov Test


### Questions:

**Q. How do we know which distribution to select from the beginning? The whole
point is that we don't know the distribution, so it seems like this is a bit of
a Catch-22.**

A. That is an acknowledged drawback of the Method of Moments. Choosing the
correct distribution has a lot to do with how effective this is.
