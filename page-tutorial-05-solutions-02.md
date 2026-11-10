# Tutorial 5 solutions: P1: Linear independence and span of vector families

PDF page 2 of 5.

[Page map](map-tutorial-05-solutions.md) | [Original PDF page](tutorial-05-solutions.pdf#page=2) | [Previous](page-tutorial-05-solutions-01.md) | [Next](page-tutorial-05-solutions-03.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
For its span,
span(S3) = {a1(0, 1, 0) + a2(−2, 2, 0) : a1, a2 ∈R} = {(−2a2, a1 + 2a2, 0) : a1, a2 ∈R} .
Note that no matter what a1 and a2 we choose, the third entry is always zero. And
any vector (x, y, 0) ∈R2 can be written as (−2a2, a1 + 2a2) by letting a2 = −x/2 and
a1 = y + x. Thus,
span(S3) = {(x, y, 0) : x, y ∈R}.
Geometrically, the set of all vectors where the z-component is zero forms a flat, two-
dimensional plane, sometimes called the xy-plane.
(iv) S4 is linearly dependent because (−2, 3, 0) = (0, 1, 0) + (−2, 2, 0), or equivalently,
(−2, 3, 0) −(0, 1, 0) −(−2, 2, 0) = (0, 0, 0).
By comparing S3 in part (iii) and S4, we see that S4 = S3 ∪{(−2, 3, 0)}. But since the
vector (−2, 3, 0) can be written as a linear combination of elements in S3, it belongs to
the span of S3, and therefore including this vector doesn’t enlarge the span. Therefore,
span(S4) = span(S3) = {(x, y, 0) : x, y ∈R}.
(v) To determine whether S5 is linearly independent, we consider
a1(1, 1, 0) + a2(0, −3, 1) + a3(2, 4, −1) = (0, 0, 0).
This is equivalent to
a1 + 2a3 = 0
a1 −3a2 + 4a3 = 0
a2 −a3 = 0
We see from the last equation that a2 = a3; plugging it to the second equation, we get
a1 + a3 = 0. Now compare it with the first equation, we get a3 = 0. Then because
a2 = a3 and a1 + a3 = 0, it must be that a1 = a2 = a3 = 0, showing that S5 is linearly
independent.
It is routine to see that
span(S5) = {a1(1, 1, 0) + a2(0, −3, 1) + a3(2, 4, −1) : a1, a2, a3 ∈R}
= {(a1 + 2a3, a1 −3a2 + 4a3, a2 −a3) : a1, a2, a3 ∈R}.
One can verify that every vector (x1, x2, x3) ∈R3 can be written as (a1 + 2a3, a1 −
3a2 + 4a3, a2 −a3) by solving the system of equations
a1 + 2a3 = x1
a1 −3a2 + 4a3 = x2
a2 −a3 = x3
and getting
a1 = −x1 + 2x2 + 6x3
a2 = x1 −x2 −2x3
a2 = x1 −x2 −3x3
Thus, span(S5) = R3.
2
```
