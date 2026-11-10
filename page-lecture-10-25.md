# Lecture 10: Equality-constraint theorem

PDF page 25 of 28; printed slide 25.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=25) | [Previous](page-lecture-10-24.md) | [Next](page-lecture-10-26.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The discussion in the previous two slides gives rise to the following result:
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable function.
Suppose
either each gj : S →R, j = 1, . . . , m, is an ane function,
or each gj : S →R, j = 1, . . . , m, is continuously dierentiable, and the set of gradients of
constraint functions {g1(x∗), . . . , gm(x∗)} is linearly independent.
If x∗∈S and it is a solution to problem
max
x∈S f (x)
s.t. gi(x) = 0 for i = 1, . . . , m,
Then there exists λ∗= (λ∗
1, . . . , λ∗
m) ∈Rm such that gi(x∗) = 0 for each i = 1, . . . , m, and
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0.
ECON 2050  Optimization III
25 / 28
```
