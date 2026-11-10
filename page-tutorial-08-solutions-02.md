# Tutorial 8 solutions: P1: Affine-inner composition, quadratic curvature and extrema; P2: Logarithmic domain and absence of extrema

PDF page 2 of 5.

[Page map](map-tutorial-08-solutions.md) | [Original PDF page](tutorial-08-solutions.pdf#page=2) | [Previous](page-tutorial-08-solutions-01.md) | [Next](page-tutorial-08-solutions-03.md)

Topics: continuity, convexity, unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
Problem 2
Calculate the critical points of the function f : C →R given by
f(x, y) = ln(8y −x2 + 4x),
and find out all its local or global extrema (i.e., maxima or minima).
Solution: Since h(z) = ln z is a strictly increasing function, by a theorem in the lecture, the
local and global maxima [minima] of g : D →R given by g(x, y) = 8y −x2 + 4x coincide
with the local and global maxima [minima] of f = h ◦g, respectively. From
∂g(x, y)
∂x
= −2x + 4 = 0
⇐⇒
x = 2
∂g(x, y)
∂y
= 8 = 0
⇐⇒
impossible
we conclude that no critical points exist.
Since C is an open set (see the graphical illustration below), every (x, y) ∈C that is not
a critical point cannot be a local extremum, and hence cannot be a global extremum either.
Thus, no local or global extremum exists.
2
```
