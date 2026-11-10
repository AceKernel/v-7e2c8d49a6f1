# Lecture 11: Lagrange global-sufficiency theorem

PDF page 16 of 25; printed slide 16.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=16) | [Previous](page-lecture-11-15.md) | [Next](page-lecture-11-17.md)

Topics: convexity, lagrange, kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable concave
function, and each gj : S →R, j = 1, . . . , m, is a continuously dierentiable convex function.
If x∗∈S and there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0,
gi(x∗) ≤0
for all i = 1, . . . , m,
λ∗
i gi(x∗) = 0
for all i = 1, . . . , m,
then x∗is a solution to problem
max
x∈S f (x)
s.t. gi(x) ≤0 for i = 1, . . . , m.
ECON 2050  Optimization IV
16 / 25
```
