# Lecture 9: Constructing a dual program

PDF page 11 of 26; printed slide 11.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=11) | [Previous](page-lecture-09-10.md) | [Next](page-lecture-09-12.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
We can formalize this process by letting y1 and y2 be the coecients of our linear combination.
We must have
y1 + y2
≥1,
3y1 + y2
≥2,
y1, y2
≥0,
and we seek to minimize 4y1 + 2y2.
We obtained another linear program!
We refer to this new linear program as the dual and the original one as the primal.
Recall that we designed the dual to serve as a method of constructing an upper bound on the
optimal value of the primal.
If (y1, y2) is feasible for the dual, and (x1, x2) is feasible for the primal, then by
construction x1 + 2x2 ≤4y1 + 2y2.
If we can nd feasible (x∗
1, x∗
2) and (y ∗
1 , y∗
2 ) that make these equal, we know we have found
the optimal values of both programs. In fact, (x ∗
1, x∗
2) = (1, 1) and (y ∗
1 , y∗
2 ) = (1/2, 1/2).
ECON 2050  Optimization II
11 / 26
```
