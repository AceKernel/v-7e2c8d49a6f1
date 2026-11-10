# Tutorial 4 solutions: P1: First-order Taylor approximation of a logarithm; P2: Chain rule along a parametrised curve

PDF page 1 of 5.

[Page map](map-tutorial-04-solutions.md) | [Original PDF page](tutorial-04-solutions.pdf#page=1) | [Next](page-tutorial-04-solutions-02.md)

Topics: chain-hessian, differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Econ 2050
Tutorial 4 Solution
Problem 1
Determine the (first-order) Taylor approximation of
f : R2
++ →R, (x, y) 7→ln(3x + 2y)
around the point a = (2, 1).
Solution: Since
∇f(x, y) =
∂f(x, y)
∂x
, ∂f(x, y)
∂y

=

3
3x + 2y,
2
3x + 2y

,
the first-order Taylor approximation around around the point a = (2, 1) equals
f(a) + ∇f(a) · (x −a) = ln(8) +
3
8, 2
8

· (x −2, y −1)
= ln(8) + 3
8(x −2) + 2
8(y −1)
= ln(8) + 3
8x + 2
8y −1
Problem 2
Suppose x(z) = z2 + 1, y(z) = ez, and
f(x, y) = 3x2
y .
Let F(z) ≡f(x(z), y(z)); calculate F ′(z) at z = 0.
Solution: We use the (generalized) chain rule to derive F ′(z):
F ′(z) = ∂f(x(z), y(z))
∂x
x′(z) + ∂f(x(z), y(z))
∂y
y′(z).
We have
∂f(x, y)
∂x
= 6x
y ,
and
∂f(x, y)
∂y
= −3x2
y2 .
1
```
