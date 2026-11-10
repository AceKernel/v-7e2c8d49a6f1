# Tutorial 4, Problem 2: Chain rule along a parametrised curve

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-04-solutions.md) | [Original PDF](tutorial-04-solutions.pdf)

Topics: chain-hessian.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-04-solutions.pdf#page=1)

```text
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

## PDF page 2

[Original page](tutorial-04-solutions.pdf#page=2)

```text
Econ 2050
Evaluating at x(z) = z2 + 1 and y(z) = ez:
∂f(x(z), y(z))
∂x
= 6(z2 + 1)
ez
,
and
∂f(x(z), y(z))
∂y
= −3(z2 + 1)2
e2z
.
Furthermore, x′(z) = 2z, and y′(z) = ez. Therefore,
F ′(z) = 12z(z2 + 1)
ez
−3(z2 + 1)2
ez
= 12z(z2 + 1) −3(z2 + 1)2
ez
.
Evaluating at z = 0 gets us
F ′(0) = 12(0)(02 + 1) −3(02 + 1)2
e0
= −3
1 = −3.
```
