# Lecture 4: Implicit function theorem with several inputs

PDF page 24 of 25; printed slide 24.

[Page map](map-lecture-04.md) | [Original PDF page](lecture-04.pdf#page=24) | [Previous](page-lecture-04-23.md) | [Next](page-lecture-04-25.md)

Topics: implicit.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Implicit function theorem: General case
Theorem
Suppose x0 ∈Rm, y0 ∈R, and G(x, y) is a continuously differentiable real-valued function
defined on an open set containing (x0, y0). If
G(x0, y0) = C
and
∂G(x0, y0)
∂y
̸= 0,
then there exists a δ > 0 and a continuously differentiable function g : Bδ(x0) →R such that
G(x, g(x)) = C for all x ∈Bδ(x0),
g(x0) = y0, and
∂g(x0)
∂xi
= −
∂G(x0, y0)
∂xi
∂G(x0, y0)
∂y
for all i = 1, . . . , m.
ECON 2050 – Basic Real Analysis IV
24 / 25
```
