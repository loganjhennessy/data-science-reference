# When to use recommender systems

Facebook, Netflix, Amazon use recommender systems. They are very
concerned with using them for economic systems.

# What the datasets look like

Lots of zeros (or question marks). Each row has thousands of features
(sometimes more). If someone on Netflix hasn't watched a movie, then
somewhere in in Netflix's database, there is an empty value for that
user for that feature.

We have to decide what to do in these situations and how to handle
these default (or zero) values.

We call this matrix (of users to features) a "utility matrix".

# How to build (from a high level)

## 1. Popularity
   - Doesn't look at the individual user at all, just at the behavior of
    users as an aggregate.
## 2. Collaborative filtering
  - Recommends based on the attributes of an item
   - For example, movies have attributes like 'director', 'cast', etc.
   - Other users' behavior is **not** considered
## 3. Content-based (a.k.a. content filtering)
   - Only consider the user's past behavior
   - Item-item or user-user similarity
## 4. Matrix factorization methods

### An aside about distance

When talking about "distance", three things must be true.

1. Dist(A, A) = 0
2. Dist(A, B) = Dist(B, A)
3. Dist(A, B) + Dist(B, C) > Dist(A, C)
