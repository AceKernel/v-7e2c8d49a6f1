# Lecture 10: Mixed equality and inequality theorem

PDF page 28 of 28; printed slide 28.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=28) | [Previous](page-lecture-10-27.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
A more general result for problems with both equality and inequality constraints:
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable function.
Suppose
either each gj : S →R, j = 1, . . . , m, is an ane function,
or each gj : S →R, j = 1, . . . , m, is continuously dierentiable, and the set of gradients of
constraint functions binding at x ∗is linearly independent.
If x∗∈S and it is a solution to problem
max
x∈S f (x)
s.t. gi(x) = 0 for i = 1, . . . , k, and gi(x) ≤0 for i = k + 1, . . . , m,
Then there exists λ∗= (λ∗
1, . . . , λ∗
m) ∈Rm such that λi ≥0 for each i = k + 1, . . . , m, and
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0,
gi(x∗) = 0 for all i = 1, . . . , k, and gi(x∗) ≤0 for all i = k + 1, . . . , m,
λ∗
i gi(x∗) = 0
for all i = k + 1, . . . , m.
ECON 2050  Optimization III
28 / 28
```
