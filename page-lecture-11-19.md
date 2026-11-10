# Lecture 11: Disk example: global optimum

PDF page 19 of 25; printed slide 19.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=19) | [Previous](page-lecture-11-18.md) | [Next](page-lecture-11-20.md)

Topics: convexity, lagrange, kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: We saw from the exercise on slide 12 that for the maximization problem
max f (x, y) = x + y
s.t.
x2 + y2 ≤2, x ≥0, y ≥0,
the only point that satises the KKT conditions is (x ∗, y∗) = (1, 1).
To conclude that (1, 1) is indeed a solution, we can
either apply the extreme value theorem like what we did in the exercise,
or note that the objective function is concave and the constraint function
g(x, y) = x2 + y2 −2 is convex, and then apply the theorem on the previous slide.
ECON 2050  Optimization IV
19 / 25
```
