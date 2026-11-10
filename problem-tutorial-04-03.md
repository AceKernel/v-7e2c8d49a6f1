# Tutorial 4, Problem 3: Implicit partial derivatives

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-04-solutions.md) | [Original PDF](tutorial-04-solutions.pdf)

Topics: implicit.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 2

[Original page](tutorial-04-solutions.pdf#page=2)

```text
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
```
