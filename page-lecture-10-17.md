# Lecture 10: Worked inequality problem

PDF page 17 of 28; printed slide 17.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=17) | [Previous](page-lecture-10-16.md) | [Next](page-lecture-10-18.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: Consider the maximization problem
max
(x1,x2)∈R2 x2
1 + x2
2
s.t.
x1 + x2 −1 ≥0.
To apply the theorem, we rst need to write the constraint as g(x1, x2) ≡1 −x1 −x2 ≤0.
One way to see that the Lagrange conditions are necessary is that the lone constraint
function is ane. One can also note that ∇g(x1, x2) = (1, 1) ̸= (0, 0) for all (x1, x2) ∈R2,
and hence {∇g(x1, x2)} is linearly independent for every (x1, x2) in the constraint set.
The Lagrange conditions are
2x1 + λ = 0
2x2 + λ = 0
λ(1 −x1 −x2) = 0
λ ≥0
1 −x1 −x2 ≤0
ECON 2050  Optimization III
17 / 28
```
