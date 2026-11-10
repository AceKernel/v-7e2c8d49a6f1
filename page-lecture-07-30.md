# Lecture 7: Paraboloid tangent-plane example

PDF page 30 of 30; printed slide 30.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=30) | [Previous](page-lecture-07-29.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: Consider f : R2 →R, (x, y) ↦→x2 + y2.
f ’s tangent plane at point (x0, y0) is given by
g(x, y) = f (x0, y0) + ∇f (x0, y0) · (x −x0, y −y0)
= f (x0, y0) + ∂f (x0, y0)
∂x
(x −x0) + ∂f (x0, y0)
∂y
(y −y0)
= x2
0 + y2
0 + 2x0(x −x0) + 2y0(y −y0)
= 2x0x + 2y0y −x2
0 −y2
0
Thus we obtain
f (x, y) −g(x, y) = x2 + y2 −(2x0x + 2y0y −x2
0 −y2
0 ) = (x −x0)2 + (y −y0)2
As f (x, y) −g(x, y) > 0 for all (x, y) ̸= (x0, y0), we conclude by the previous theorem
that f is strictly convex.
ECON 2050 – Convexity
30 / 30
```
