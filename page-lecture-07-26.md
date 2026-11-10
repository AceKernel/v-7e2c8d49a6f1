# Lecture 7: First-order characterisation of convexity and concavity

PDF page 26 of 30; printed slide 26.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=26) | [Previous](page-lecture-07-25.md) | [Next](page-lecture-07-27.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
First-order conditions for convexity/concavity
Theorem (compare SB Thm 21.2, 21.3)
If S ⊆Rn is open and convex and f : S →R continuously differentiable, then f is
concave if and only if
∀x, x0 ∈S :
f (x) −f (x0) ≤∇f (x0) · (x −x0)
(6)
strictly concave if and only if inequality (6) is strict for all x ̸= x0.
convex if and only if
∀x, x0 ∈S :
f (x) −f (x0) ≥∇f (x0) · (x −x0)
(7)
strictly convex if and only if inequality (7) is strict for all x ̸= x0.
ECON 2050 – Convexity
26 / 30
```
