# Tutorial 4 solutions: P2: Chain rule along a parametrised curve; P3: Implicit partial derivatives; P4: Tangent lines to implicit level curves

PDF page 2 of 5.

[Page map](map-tutorial-04-solutions.md) | [Original PDF page](tutorial-04-solutions.pdf#page=2) | [Previous](page-tutorial-04-solutions-01.md) | [Next](page-tutorial-04-solutions-03.md)

Topics: chain-hessian, graphs, implicit.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
Problem 3
Suppose that it follows from the implicit function theorem that, in a neighborhood of
(x0, y0, z0), z is implicitly defined by the equation zex + ey −yez = 0 as a function of x and
y. Compute the partial derivatives ∂z
∂x and ∂z
∂y at the point (x0, y0).
Solution: The partial derivatives of f : R3 →R, (x, y, z) 7→zex +ey −yez at (x0, y0, z0) are:
∂f(x0, y0, z0)
∂x
= z0ex0
∂f(x0, y0, z0)
∂y
= ey0 −ez0
∂f(x0, y0, z0)
∂z
= ex0 −y0ez0
We must have ∂f(x0, y0, z0)
∂z
̸= 0, otherwise, the implicit function theorem would not apply.
Using the implicit function theorem, we obtain:
∂z(x0, y0)
∂x
= −
∂f(x0,y0,z0)
∂x
∂f(x0,y0,z0)
∂z
= −
z0ex0
ex0 −y0ez0
∂z(x0, y0)
∂y
= −
∂f(x0,y0,z0)
∂y
∂f(x0,y0,z0)
∂z
= −ey0 −ez0
ex0 −y0ez0 =
ez0 −ey0
ex0 −y0ez0
Problem 4
Obtain an equation of the tangent line to the level curve of f : R2 →R at the point
1. (x0, y0) = (1, 1) if f(x, y) = xexy
2. (x0, y0) = (−1, 2) if f(x, y) = y −x2
2
```
