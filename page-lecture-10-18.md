# Lecture 10: Binding and slack case procedure

PDF page 18 of 28; printed slide 18.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=18) | [Previous](page-lecture-10-17.md) | [Next](page-lecture-10-19.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Rule of thumb: The most convenient way of solving the Lagrange conditions is usually to start
from complementary slackness.
If λ = 0, then from the rst two equalities we see that x1 = x2 = 0, violating
1 −x1 −x2 ≤0. Thus, λ > 0.
Consequently, complementary slackness requires x1 + x2 = 1.
From the rst two equalities (2x1 + λ = 0 and 2x2 + λ = 0), we see that x1 = x2 = −λ/2.
Together with x1 + x2 = 1, we get x1 = x2 = 1/2 and λ = −1. But λ > 0, a contradiction.
Thus, there is no point that satises the Lagrange conditions for this problem.
Because the Lagrange conditions are necessary, that is, every solution must satisfy the
Lagrange conditions, the maximization problem has no solution.
ECON 2050  Optimization III
18 / 28
```
