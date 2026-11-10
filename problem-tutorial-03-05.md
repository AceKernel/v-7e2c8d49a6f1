# Tutorial 3, Problem 5: Chain rule for logarithmic and square-root functions

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-03-solutions.md) | [Original PDF](tutorial-03-solutions.pdf)

Topics: differentiation; chain-hessian.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 4

[Original page](tutorial-03-solutions.pdf#page=4)

```text
Problem 5 (Extra Practice Problem)
For each of the following functions f, calculate the partial derivatives, and eval-
uate them at the point (1, 1).
(a) f : R2 →R, (x, y) 7→ln(x2 + y2 + 1)
(b) f : R2
++ →R, (x, y) 7→
p
xy + y3
Solution:
(a) To find ∂f(x,y)
∂x
, we treat y as a constant, and use the chain rule:
1. Take the derivative of the outer function, ln(u), where u ≡x2 +y2 +1, which
is 1
u.
4
```

## PDF page 5

[Original page](tutorial-03-solutions.pdf#page=5)

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
