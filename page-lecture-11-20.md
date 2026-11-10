# Lecture 11: Affine equalities for global sufficiency

PDF page 20 of 25; printed slide 20.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=20) | [Previous](page-lecture-11-19.md) | [Next](page-lecture-11-21.md)

Topics: convexity, lagrange, kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
With equality constraints, we need to further assume that the constraint functions are ane.
Otherwise, the constraint set need not be convex.
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable concave
function, and each gj : S →R, j = 1, . . . , m, is an ane function.
If x∗∈S and there exists λ∗= (λ∗
1, . . . , λ∗
m) ∈Rm such that gi(x∗) = 0 for each i = 1, . . . , m,
and
∇f (x∗) −λ1∇g1(x∗) −λ2∇g2(x∗) −· · · −λm∇gm(x∗) = 0,
then x∗is a solution to problem
max
x∈S f (x)
s.t. gi(x) = 0 for i = 1, . . . , m.
ECON 2050  Optimization IV
20 / 25
```
