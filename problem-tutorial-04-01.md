# Tutorial 4, Problem 1: First-order Taylor approximation of a logarithm

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-04-solutions.md) | [Original PDF](tutorial-04-solutions.pdf)

Topics: differentiation.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-04-solutions.pdf#page=1)

```text
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
```
