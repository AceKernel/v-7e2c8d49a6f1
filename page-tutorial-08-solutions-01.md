# Tutorial 8 solutions: P1: Affine-inner composition, quadratic curvature and extrema

PDF page 1 of 5.

[Page map](map-tutorial-08-solutions.md) | [Original PDF page](tutorial-08-solutions.pdf#page=1) | [Next](page-tutorial-08-solutions-02.md)

Topics: convexity, unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Tutorial 8 Solution
Problem 1
In lecture 7, we learned about a result that if f = h ◦g, where h is increasing and
convex, and g is convex, then f is also convex. We have also seen examples where the
“outer function” h is convex but not increasing and therefore the composition fails to be
convex.
However, if the “inner function” g is not just convex, but affine, then even if the “outer
function” h is convex but not increasing, the composition h ◦g is still convex.
(a) Prove the fact stated in the second paragraph; that is, if g : S →R is affine and h : R →
R is convex, where S ⊆Rn, then the composition f ≡h ◦g is convex. (Similarly, if g is
affine and h is concave, then the composition h ◦g is concave.)
(b) Use the fact in part (a) to show that
• f1(x, y) = (y −x)2 is convex; and
• f2(x, y) = −x2 −5y2 −4xy is concave.
(c) Find the global minima of f1(x, y).
(d) Find the global maxima of f2(x, y).
Solution:
(a) We need to show that f = h◦g is convex; that is, for any x1, x2 ∈S and every λ ∈[0, 1],
f (λx1 + (1 −λ)x2) ≤λf (x1) + (1 −λ)f (x2) ,
or equivalently,
h(g (λx1 + (1 −λ)x2)) ≤λh(g (x1)) + (1 −λ)h(g((x2)).
(1)
Since g is affine, it is both convex and concave, meaning that for any x1, x2 ∈S and
every λ ∈[0, 1],
g (λx1 + (1 −λ)x2) = λg (x1) + (1 −λ)g (x2) ;
thus,
h(g (λx1 + (1 −λ)x2)) = h(λg (x1) + (1 −λ)g (x2)).
(2)
Since h is convex, for any z1, z2 ∈R and every λ ∈[0, 1],
h (λz1 + (1 −λ)z2) ≤λh (z1) + (1 −λ)h (z2) .
Taking z1 ≡g(x1) and z2 ≡g(x2), inequality (2) implies
h(g (λx1 + (1 −λ)x2)) = h(λg (x1)+(1−λ)g (x2)) ≤λh(g (x1))+(1−λ)h(g((x2)),
which yields the desired inequality (1). Thus, f = h ◦g is a convex function.
1
```
