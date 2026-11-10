# Lecture 11: KKT necessity and constraint qualification

PDF page 7 of 25; printed slide 7.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=7) | [Previous](page-lecture-11-06.md) | [Next](page-lecture-11-08.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem
Let S be an open subset of Rn, and let f : S →R be continuously dierentiable functions.
Suppose
either each gj : S →R, j = 1, . . . , m, is an ane function,
or each gj : S →R, j = 1, . . . , m, is continuously dierentiable, and the set of gradients of
constraint functions (including the nonnegative constraints) binding at x ∗is linearly
independent.
If x∗∈S and it is a solution to problem
max
x∈S f (x)
s.t. gj(x) ≤0 for j = 1, . . . , m, and x ≥0.
Then there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that (x∗, λ∗) satises the Karush-Kuhn-Tucker
(KKT) conditions.
ECON 2050  Optimization IV
7 / 25
```
