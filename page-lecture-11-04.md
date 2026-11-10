# Lecture 11: Reducing the stationarity conditions

PDF page 4 of 25; printed slide 4.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=4) | [Previous](page-lecture-11-03.md) | [Next](page-lecture-11-05.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The rst two equalities can be written as
∂f (x1, x2)
∂x1
−λ∂g(x1, x2)
∂x1
= −ν1,
∂f (x1, x2)
∂x2
−λ∂g(x1, x2)
∂x2
= −ν2
(△)
Since ν1, ν2 ≥0, (△) is equivalent to
∂f (x1, x2)
∂x1
−λ∂g(x1, x2)
∂x1
≤0
∂f (x1, x2)
∂x2
−λ∂g(x1, x2)
∂x2
≤0
⇐⇒
∇f (x1, x2) −λ∇g(x1, x2) ≤0.
Again by (△), the two complementary slackness conditions, ν1x1 = 0 and ν2x2 = 0, become
x1
(︃∂f (x1, x2)
∂x1
−λ∂g(x1, x2)
∂x1
)︃
= 0
and
x2
(︃∂f (x1, x2)
∂x2
−λ∂g(x1, x2)
∂x2
)︃
= 0
Bringing back the other four conditions, g(x1, x2) ≤0, λ ≥0, x1 ≥0, x2 ≥0, and
λg(x1, x2) = 0, we obtained a new set of conditions without the Lagrange multipliers on the
nonnegativity constraints, ν1 and ν2.
ECON 2050  Optimization IV
4 / 25
```
