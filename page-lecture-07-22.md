# Lecture 7: Convexity equivalences for epigraphs and hypographs

PDF page 22 of 30; printed slide 22.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=22) | [Previous](page-lecture-07-21.md) | [Next](page-lecture-07-23.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Proposition
Let S ⊆Rn be convex. A function f : S →R is
concave if and only if its hypograph is a convex set.
convex if and only if its epigraph is a convex set.
Proof (first part): “⇒”: Suppose that f is concave. We want to show that hyp(f ) is a convex
set.
Let (x1, y1), (x2, y2) ∈hyp(f ), and λ ∈[0, 1]. We have to show that
λ(x1, y1) + (1 −λ)(x2, y2) ∈hyp(f ).
Since (x1, y1) ∈hyp(f ), y1 ≤f (x1) and thus
λy1 ≤λf (x1)
(4)
Since (x2, y2) ∈hyp(f ), y2 ≤f (x2) and thus
(1 −λ)y2 ≤(1 −λ)f (x2)
(5)
ECON 2050 – Convexity
22 / 30
```
