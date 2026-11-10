# Lecture 9: General dual and weak duality

PDF page 12 of 26; printed slide 12.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=12) | [Previous](page-lecture-09-11.md) | [Next](page-lecture-09-13.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Duality
More generally, consider the standard form of a linear programming problem
max c · x
s.t. Ax ≤b, x ≥0.
(P)
Taking a linear combination of the constraints with weights y = (y1, . . . , ym) can be written as
yA; since we need to nd an upper bound, it must be that yA ≥c.
Since x ≥0, we have yAx ≥c · x.
Then because Ax ≤b, c · x ≤yAx ≤y · b. Thus, y · b is an upper bound on objective
function value.
Therefore, the problem of nding the smallest such upper bound is
min y · b
s.t. yA ≥c, y ≥0.
(D)
We call problem (D) the dual and problem (P) the primal.
Denote the optimal values of (P) and (D) by V and W , respectively.
Since c · x ≤y · b, we have V ≤W ; this is known as weak duality.
ECON 2050  Optimization II
12 / 26
```
