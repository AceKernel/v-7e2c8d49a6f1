# Tutorial 8, Problem 1: Affine-inner composition, quadratic curvature and extrema

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-08-solutions.md) | [Original PDF](tutorial-08-solutions.pdf)

Topics: convexity; unconstrained.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-08-solutions.pdf#page=1)

```text
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

## PDF page 2

[Original page](tutorial-08-solutions.pdf#page=2)

```text
ECON 2050
S2 2026
(b) f1(x, y) = (y −x)2 is convex because f1 = h1 ◦g1, where h1(z) = z2 is convex and
g1(x, y) = x −y is linear (and therefore affine).
For f2, note that
f2(x, y) = −x2 −5y2 −4xy = −(x2 + 4xy + 4y2) −y2 = −(x + 2y)2 −y2.
By the fact we proved in part (a), we know that g2(x, y) := −(x + 2y)2 is concave
because g2 = u ◦v, where u(z) = −z2 is concave and v(x, y) = x + 2y is linear (and
therefore affine). Also, it is not difficult to see (for example, Tutorial 7 problem 2) that
h2(x, y) = −y2 is concave. Then since f2(x, y) = g2(x, y)+h2(x, y), f2(x, y) is concave.
(c) From
∂f1(x, y)
∂x
= −2(y −x) = 0
⇐⇒
y = x
∂f1(x, y)
∂y
= 2(y −x) = 0
⇐⇒
y = x
we see that (x, y) ∈R2 is a critical point of f1 if and only if y = x. By part (b), f is
convex, and therefore all the critical points, namely the points on the line determined
by y = x, are global minima.
(d) From
∂f2(x, y)
∂x
= −2x −4y = 0
∂f2(x, y)
∂y
= −10y −4x = 0
we deduce that the only critical point of f is (x∗, y∗) = (0, 0). Since we determined in
part (b) that f2 is concave, (x∗, y∗) = (0, 0) is the unique global maximum.
```
