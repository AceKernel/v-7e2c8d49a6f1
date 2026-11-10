# Tutorial 3 solutions: P5: Chain rule for logarithmic and square-root functions

PDF page 5 of 5.

[Page map](map-tutorial-03-solutions.md) | [Original PDF page](tutorial-03-solutions.pdf#page=5) | [Previous](page-tutorial-03-solutions-04.md)

Topics: chain-hessian, differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
2. Multiply by the derivative of the inner function with respect to x, which is
∂(x2+y2+1)
∂x
= 2x.
Putting it together, the partial derivative with respect to x is
∂f(x, y)
∂x
=
1
x2 + y2 + 1 · (2x) =
2x
x2 + y2 + 1.
Similarly, the partial derivative with respect to y is
∂f(x, y)
∂y
=
2y
x2 + y2 + 1.
(b) To find ∂f(x,y)
∂x
, we treat y as a constant, and use the chain rule:
1. Take the derivative of the outer function, √u, where u ≡xy + y3, which is
1
2√u.
2. Multiply by the derivative of the inner function with respect to x, which is
∂(xy+y3)
∂x
= y.
Putting it together, the partial derivative with respect to x is
∂f(x, y)
∂x
=
1
2
p
xy + y3 · (y) =
y
2
p
xy + y3.
Similarly, the partial derivative with respect to y is
∂f(x, y)
∂y
=
x + 3y2
2
p
xy + y3.
5
```
