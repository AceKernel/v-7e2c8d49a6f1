# Lecture 10: Feasible-direction linearisation

PDF page 7 of 28; printed slide 7.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=7) | [Previous](page-lecture-10-06.md) | [Next](page-lecture-10-08.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Suppose x∗∈S is a solution to the non-linear program
max
x∈S f (x)
subject to
gi(x) ≤0 for all i = 1, . . . , m;
denote the constraint set by
C = {x ∈S : gi(x) ≤0 for all i = 1, . . . , m}.
Then for any x ∈C, f (x∗) ≥f (x).
Because f is continuously dierentiable, around x ∗we can approximate f by its (rst-order)
Taylor approximation (see lecture 3 slide 24):
f (x∗+ h) ≈f (x∗) + ∇f (x∗) · h.
Similarly, we can approximate each of the constraint functions gi around x∗:
gi(x∗+ h) ≈gi(x∗) + ∇gi(x∗) · h.
ECON 2050  Optimization III
7 / 28
```
