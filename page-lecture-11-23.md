# Lecture 11: Linear programs as KKT systems

PDF page 23 of 25; printed slide 23.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=23) | [Previous](page-lecture-11-22.md) | [Next](page-lecture-11-24.md)

Topics: duality, kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Consider a linear programming problem max{c · x : Ax ≤b, x ≥0}. To be more concrete, let
c = (c1, c2),
A =
(︃a11
a12
a21
a22
)︃
,
and
b = (b1, b2);
that is, the problem can be written as
max
(x1,x2)∈R2 c1x1 + c2x2
s.t.
a11x1 + a12x2 ≤b1
a21x1 + a22x2 ≤b2
x1 ≥0, x2 ≥0
Its dual is min{y · b : yA ≥c, y ≥0}, which can be written as
min
(y1,y2)∈R2 b1y1 + b2y2
s.t.
a11y1 + a21y2 ≥c1
a12y1 + a22y2 ≥c2
y1 ≥0, y2 ≥0
ECON 2050  Optimization IV
23 / 25
```
