# Lecture 11: Matching LP and KKT conditions

PDF page 24 of 25; printed slide 24.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=24) | [Previous](page-lecture-11-23.md) | [Next](page-lecture-11-25.md)

Topics: duality, kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
KKT for linear programming problems
By the result on slide 22, since the objective function is linear and therefore concave, the
solutions of this problem are precisely the points satisfying the KKT conditions.
The KKT conditions are
c1 −λ1a11 −λ2a21 ≤0,
x1(c1 −λ1a11 −λ2a21) = 0,
x1 ≥0;
c2 −λ1a12 −λ2a22 ≤0,
x2(c2 −λ1a12 −λ2a22) = 0,
x2 ≥0;
a11x1 + a12x2 −b1 ≤0,
λ1(a11x1 + a12x2 −b1) = 0,
λ1 ≥0;
a21x1 + a22x2 −b2 ≤0,
λ2(a21x1 + a22x2 −b2) = 0,
λ2 ≥0.
Observe that (by changing λ1, λ2 to y1, y2) the KKT conditions are precisely the dual
constraints, primal constraints, and the complementary slackness conditions.
ECON 2050  Optimization IV
24 / 25
```
