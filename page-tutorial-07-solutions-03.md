# Tutorial 7 solutions: P3: Convexity of intersecting constraint sets; P4: Convexity and concavity by composition; P5: Strict convexity of a square from the definition

PDF page 3 of 5.

[Page map](map-tutorial-07-solutions.md) | [Original PDF page](tutorial-07-solutions.pdf#page=3) | [Previous](page-tutorial-07-solutions-02.md) | [Next](page-tutorial-07-solutions-04.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
Problem 4
Analyze whether the following functions are concave or convex.
1. f1(x, y) = 4x2 + e2y2.
2. f2(x, y) = ln(3x + 2y).
Solution:
1. Observe that f1(x, y) = g1(x) + h1(y), where g1(x) = 4x2, and h1(y) = e2y2. Now
g1(x) is convex, and h1(y) = m ◦n, where m(u) = eu is increasing and convex, and
n(y) = 2y2 is convex. Thus, both g1 and h1 are convex; by the result we proved in
Problem 2, f1(x, y) is also convex.
2. f2(x, y) = ln(3x + 2y) is concave because f2 = h2 ◦g2, where h2(u) = ln u is an
increasing concave function, and g2(x, y) = 3x + 2y is linear and hence concave.
Problem 5
Prove from the definition of a strictly convex function and without using any theorem
about convex functions that f(x) = x2 is strictly convex.
3
```
