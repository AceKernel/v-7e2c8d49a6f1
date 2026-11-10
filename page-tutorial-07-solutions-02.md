# Tutorial 7 solutions: P2: Convexity of a separable sum; P3: Convexity of intersecting constraint sets

PDF page 2 of 5.

[Page map](map-tutorial-07-solutions.md) | [Original PDF page](tutorial-07-solutions.pdf#page=2) | [Previous](page-tutorial-07-solutions-01.md) | [Next](page-tutorial-07-solutions-03.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
and
h(λy′ + (1 −λ)y′′) ≤λh(y′) + (1 −λ)h(y′′).
Thus,
f(λ(x′, y′) + (1 −λ)(x′′, y′′)) = g(λx′ + (1 −λ)x′′) + h(λy′ + (1 −λ)y′′)
≤λg(x′) + (1 −λ)g(x′′) + λh(y′) + (1 −λ)h(y′′)
= λ[g(x′) + h(y′)] + (1 −λ)[g(x′′) + h(y′′)]
= λf(x′, y′) + (1 −λ)f(x′′, y′′)
By definition, f(x, y) is convex.
Problem 3
Show that the following sets are convex.
1. S = {(x, y) ∈R2 : y ≥x, x2 + y2 ≤4}
2. T = {(x, y) ∈R2 : y ≥x2, y ≤4}
Solution:
1. We observe that
• S1 = {(x, y) ∈R2 : y ≥x} is convex because S1 = epi(f1), where f1 : R →R
is given by f1(x) = x is a convex function (because it’s linear, and hence affine;
affine functions are both convex and concave).
(Alternatively, one may note that S1 = {(x, y) ∈R2 : x −y ≤0}. One can
use the result we proved in Problem 2 to show that fa(x, y) = x −y is a convex
function (let g(x) = x and h(y) = −y) and then apply the result we proved in
Problem 1.)
• S2 = {(x, y) ∈R2 : x2 + y2 ≤4} is convex by the result in Problem 1 because
we proved in lecture 7 that the function f2(x, y) = x2 + y2 is convex.
Thus, since S = S1∩S2 and since the intersection of convex sets is convex, S is convex.
Graphically,
2
```
