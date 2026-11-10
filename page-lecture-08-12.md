# Lecture 8: Concavity and convexity give global sufficiency

PDF page 12 of 25; printed slide 12.

[Page map](map-lecture-08.md) | [Original PDF page](lecture-08.pdf#page=12) | [Previous](page-lecture-08-11.md) | [Next](page-lecture-08-13.md)

Topics: convexity, unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem (Sucient conditions for global extrema)
Let D ⊆Rn be convex, f : D →R be a dierentiable function. Then:
1 Suppose f is concave, then x∗is a (global) maximum of f if it is a critical point of f .
2 Suppose f is convex, then x∗is a (global) minimum of f if it is a critical point of f .
Proof: We only prove part 1; part 2 can be proved analogously. Since f is concave,
f (y) −f (x) ≤∇f (x) · (y −x),
∀x, y ∈D
(by the theorem on lecture 7 slide 26). If x ∗is a critical point of f then ∇f (x∗) = 0, meaning
that for all x ∈D,
f (x) −f (x∗) ≤0 · (x −x∗) = 0,
which is equivalent to f (x) ≤f (x∗) for all x ∈D. Hence x∗is a global maximum of f .
ECON 2050  Optimization I
12 / 25
```
