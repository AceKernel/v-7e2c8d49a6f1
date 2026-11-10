# Lecture 10: Linear-independence constraint qualification

PDF page 15 of 28; printed slide 15.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=15) | [Previous](page-lecture-10-14.md) | [Next](page-lecture-10-16.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
If some of the constraint functions are not ane, as long as the set of gradients of constraint
functions binding at x∗is linearly independent, we also have no trouble:
Theorem
Let S be an open subset of Rn, and let f : S →R and gj : S →R, j = 1, . . . , m be
continuously dierentiable functions. Suppose x ∗∈S is a solution to the problem
max
x∈S f (x)
s.t. gi(x) ≤0 for i = 1, . . . , m,
and suppose the rst k ≤m constraints are binding, and the other m −k constraints are slack.
If the set of gradients of the binding constraints, {∇g1(x∗), . . . , ∇gk(x∗)}, is linearly
independent, then there exists λ∗= (λ∗
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
15 / 28
```
