# Lecture 4: Implicit-derivative example

PDF page 22 of 25; printed slide 22.

[Page map](map-lecture-04.md) | [Original PDF page](lecture-04.pdf#page=22) | [Previous](page-lecture-04-21.md) | [Next](page-lecture-04-23.md)

Topics: implicit, graphs.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: Consider the equation x2 −3xy + y3 = 7 around the point (x0, y0) = (4, 3).
Consider the level curve of level 7 of the function G(x, y) = x2 −3xy + y3. One can show that
∂G(x, y)
∂x
= 2x −3y,
and
∂G(x, y)
∂y
= −3x + 3y2;
because both partial derivatives are continuous, G must be continuously differentiable.
Moreover, G(4, 3) = 7 and ∂G(4,3)
∂y
= 15 ̸= 0.
Then by the implicit function theorem, one can write y as a continuously differentiable
function of x, denoted by g(x), around (4, 3), and
g′(4) = −
∂G(4,3)
∂x
∂G(4,3)
∂y
= 1
15.
We can also write down the tangent line h to the level curve at the point (x0, y0) = (4, 3):
h(x) = y0 + g′(x0)(x −x0) = 3 + 1
15(x −4) = 1
15x + 1
3.
ECON 2050 – Basic Real Analysis IV
22 / 25
```
