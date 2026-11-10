# Tutorial 4 solutions: P5: Hessian calculations; P6: Implicit total derivative on a sphere

PDF page 5 of 5.

[Page map](map-tutorial-04-solutions.md) | [Original PDF page](tutorial-04-solutions.pdf#page=5) | [Previous](page-tutorial-04-solutions-04.md)

Topics: chain-hessian, implicit.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Econ 2050
Problem 6 (Extra Practice Problem)
Suppose that it follows from the implicit function theorem that, in a neighborhood of
(x0, y0, z0), z is implicitly defined by the equation x2 + y2 + z2 = a2 as a function of x and
y. Compute the total derivative Dz(x0, y0).
Solution: If we let f : R3 →R, (x, y, z) 7→x2 + y2 + z2 −a2 then the equation above is
equivalent to f(x, y, z) = 0. We have
∂f(x, y, z)
∂x
= 2x
∂f(x, y, z)
∂y
= 2y
∂f(x, y, z)
∂z
= 2z
(Since all partial derivatives of f are continuous, f is continuously differentiable.) Since the
implicit function theorem applied, ∂f(x0,y0,z0)
∂z
= 2z0 ̸= 0. By the implicit function theorem,
∂z(x0, y0)
∂x
= −
∂f(x0,y0,z0)
∂x
∂f(x0,y0,z0)
∂z
= −2x0
2z0
= −x0
z0
∂z(x0, y0)
∂y
= −
∂f(x0,y0,z0)
∂y
∂f(x0,y0,z0)
∂z
= −2y0
2z0
= −y0
z0
Therefore, Dz(x0, y0) = ∇z(x0, y0) =

−x0
z0
, −y0
z0

.
(Alternatively, from Df(x0, y0, z0) · (dx, dy, dz) = 0 we obtain
(2x0, 2y0, 2z0) · (dx, dy, dz) = 2x0dx + 2y0dy + 2z0dz = 0
or
dz = −2x0
2z0
dx −2y0
2z0
dy = −x0
z0
dx −y0
z0
dy,
and we can see that Dz(x0, y0) =

−x0
z0
, −y0
z0

.)
5
```
