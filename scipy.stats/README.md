# Probability distributions

All of the probability distributions in scipy.stats follow the same basic
interface, which makes it easy to design code that uses different distributions
interchangeably. However, it does sometimes make it difficult to understand
exactly what is going on under the hood.

There are a few parameters that are important to understand for any
distribution. They are:

- Location
- Scale
- Rate
- Shape

**Location** is one of the more trivial parameters. It just slides the
distribution left and right along the x-axis.

**Scale** is a little more interesting. In the case of the normal distribution,
this is the variance. So it can be thought of as something that will stretch
out or compress the distribution along the x-axis.

**Rate** is just a special case of scale where it is more natural to use a rate
to specify the behavior of the distribution. In scipy.stats, this ends up being
1 / scale.

**Shape** is the most complicated and can be just about anything. Different
distributions may or may not have shape parameters, and some have multiple.
