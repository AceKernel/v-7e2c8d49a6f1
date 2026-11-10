# Lecture 11: Reduced KKT global sufficiency

PDF page 18 of 25; printed slide 18.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=18) | [Previous](page-lecture-11-17.md) | [Next](page-lecture-11-19.md)

Topics: convexity, lagrange, kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
An analogous result can be obtained for points satisfying the KKT conditions.
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable concave
function, and each gj : S →R, j = 1, . . . , m, is a continuously dierentiable convex function.
If x∗∈S and there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) ≤0,
x∗
i
(︃∂g1(x∗)
∂xi
−λ∗
2
∂g2(x∗)
∂xi
−· · · −λ∗
m
∂gm(x∗)
∂xi
)︃
= 0
for all i = 1, . . . , n,
gj(x∗) ≤0
for all j = 1, . . . , m,
λ∗
j gj(x∗) = 0
for all j = 1, . . . , m,
then x∗is a solution to problem
max
x∈S f (x)
s.t. gi(x) ≤0 for i = 1, . . . , m, and x ≥0.
ECON 2050  Optimization IV
18 / 25
```
