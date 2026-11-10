# Lecture 10: Necessary conditions with affine constraints

PDF page 13 of 28; printed slide 13.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=13) | [Previous](page-lecture-10-12.md) | [Next](page-lecture-10-14.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Necessary conditions
Thankfully, when the constraint functions are all ane (like in a linear program, although the
objective function can be non-linear), we don't have to worry:
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable function, and
each gj : S →R, j = 1, . . . , m, is an ane function. If x∗∈S and it is a solution to problem
max
x∈S f (x)
s.t. gi(x) ≤0 for i = 1, . . . , m,
then there exists λ∗= (λ∗
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
for all i = 1, . . . , m.
ECON 2050  Optimization III
13 / 28
```
