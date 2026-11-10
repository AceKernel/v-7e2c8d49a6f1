# Lecture 7: Convex-set example

PDF page 6 of 30; printed slide 6.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=6) | [Previous](page-lecture-07-05.md) | [Next](page-lecture-07-07.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: T =
{︁
(x, y) ∈R2 : x + 2y ≤3
}︁
is convex: Let (x′, y′), (x′′, y′′) ∈T and λ ∈[0, 1].
We need to show that
λ(x′, y′) + (1 −λ)(x′′, y′′) = (λx′ + (1 −λ)x′′, λy′ + (1 −λ)y′′) ∈T,
or, equivalently, that
(λx′ + (1 −λ)x′′) + 2(λy′ + (1 −λ)y′′) ≤3.
(1)
But (x′, y′) ∈T implies x′ + 2y′ ≤3 and thus
λ(x′ + 2y′) ≤3λ,
(2)
and (x′′, y′′) ∈T implies x′′ + 2y′′ ≤3 and thus
(1 −λ)(x′′ + 2y′′) ≤3(1 −λ).
(3)
Adding up the two inequalities (2) and (3), we obtain (1).
ECON 2050 – Convexity
6 / 30
```
