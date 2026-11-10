# Lecture 6: No-arbitrage condition

PDF page 21 of 26; printed slide 21.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=21) | [Previous](page-lecture-06-20.md) | [Next](page-lecture-06-22.md)

Topics: Cones, Farkas and feasibility.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
If p > 0 is a vector of asset prices, we can state the no arbitrage condition algebraically as
follows:
yA ≥0 ⇒y · p ≥0
Equivalently, the system [yA ≥0 and y · p < 0] must have no solution.
From the Farkas lemma, there must exist a non-negative vector π ∈Rn
+ such that p = Aπ.
Scaling if necessary, π can be interpreted as a probability vector (i.e., ∑︁m
j=1 πi = 1) that
specifies the chance of each scenario realizes.
That is, πj is the chance (or probability) of the scenario j for each j = 1, . . . , n.
Therefore, this condition specifies that there exist chances of all scenarios (or, more
formally, a probability distribution over scenarios) under which every asset’s expected
value is equal to its price (in other words, every investment has an expected return of
zero).
An investor who using these chances would conclude that the assets are fairly priced.
ECON 2050 – Linear Algebra II
21 / 26
```
