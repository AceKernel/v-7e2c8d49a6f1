# Lecture 4: Two-variable implicit function theorem

PDF page 19 of 25; printed slide 19.

[Page map](map-lecture-04.md) | [Original PDF page](lecture-04.pdf#page=19) | [Previous](page-lecture-04-18.md) | [Next](page-lecture-04-20.md)

Topics: implicit, graphs.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem (Implicit function theorem)
Suppose G(x, y) is a continuously differentiable real-valued function defined on an open set
containing (x0, y0). If G(x0, y0) = C, and
∂G(x0, y0)
∂y
̸= 0,
then there exists a δ > 0 and a continuously differentiable function g : Bδ(x0) →R such that
G(x, g(x)) = C for all x ∈Bδ(x0),
g(x0) = y0, and
g′(x0) = −
∂G(x0, y0)
∂x
∂G(x0, y0)
∂y
.
Intuitively, if the assumptions of the theorem hold, even though y cannot be isolated in the
original equation G(x, y) = C, the derivative of y with respect to x around the point (x0, y0)
can be isolated in terms of the partial derivatives of G.
ECON 2050 – Basic Real Analysis IV
19 / 25
```
