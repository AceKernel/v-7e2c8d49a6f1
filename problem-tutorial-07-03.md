# Tutorial 7, Problem 3: Convexity of intersecting constraint sets

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-07-solutions.md) | [Original PDF](tutorial-07-solutions.pdf)

Topics: convexity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 2

[Original page](tutorial-07-solutions.pdf#page=2)

```text
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

## PDF page 3

[Original page](tutorial-07-solutions.pdf#page=3)

```text
ECON 2050
S2 2026
2. We observe that
• T1 = {(x, y) ∈R2 : y ≥x2} is convex because T1 = epi(g1), where g1(x) = x2
is a convex function (one can prove it by taking second derivative to get g′′
1(x) =
2 > 0, or prove it using definition as in Problem 5).
(Alternatively, one may note that T1 = {(x, y) ∈R2 : x2 −y ≤0}. One can
use the result we proved in Problem 2 to show that ga(x, y) = x2 −y is a convex
function (let g(x) = x2 and h(y) = −y), and then apply the result in Problem 1.)
• T2 = {(x, y) ∈R2 : y ≤4} is convex by Problem 1 because g2(x, y) = y is a
convex function by the result we proved in Problem 2.
Thus, since T = T1∩T2 and since the intersection of convex sets is convex, T is convex.
Graphically,
```
