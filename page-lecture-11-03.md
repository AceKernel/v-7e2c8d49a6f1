# Lecture 11: Explicit multipliers for nonnegativity

PDF page 3 of 25; printed slide 3.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=3) | [Previous](page-lecture-11-02.md) | [Next](page-lecture-11-04.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
To start with, consider a constrained maximization problem
max
(x1,x2)∈R2 f (x1, x2)
subject to
g(x1, x2) ≤0, x1 ≥0, x2 ≥0.
We could let n1(x1, x2) = −x1 and n2(x1, x2) = −x2, and the problem becomes
max
(x1,x2)∈R2 f (x1, x2)
subject to
g(x1, x2) ≤0, n1(x1, x2) ≤0, n2(x1, x2) ≤0.
The Lagrange conditions for this problem are
∂f (x1, x2)
∂x1
−λ∂g(x1, x2)
∂x1
+ ν1 = 0
∂f (x1, x2)
∂x2
−λ∂g(x1, x2)
∂x2
+ ν2 = 0
g(x1, x2) ≤0, λ ≥0, x1 ≥0, x2 ≥0
λg(x1, x2) = 0, ν1x1 = 0, ν2x2 = 0
ECON 2050  Optimization IV
3 / 25
```
