# Lecture 10: Equality-constraint example

PDF page 27 of 28; printed slide 27.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=27) | [Previous](page-lecture-10-26.md) | [Next](page-lecture-10-28.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: Consider the maximization problem
max
(x1,x2)∈R2 f (x1, x2) = −2x2
1 −3x2
2
s.t.
g(x1, x2) = x1 + x2 −1 = 0.
We can either use the fact that g is ane, or to notice that ∇g(x1, x2) = (1, 1) ̸= (0, 0)
for all (x1, x2) ∈R2, and therefore {∇g(x1, x2)} is linearly independent for every (x, y) in
the constraint set, to conclude that the Lagrange conditions are necessary.
The Lagrange conditions are
−4x1 + λ = 0
−6x2 + λ = 0
x1 + x2 −1 = 0
From the rst two equations we get λ = 4x1 = 6x2, and therefore x1 = 3
2x2.
Plugging into the third equation (the equality constraint), we get the unique solution
(x∗
1, x∗
2, λ∗) = (3/5, 2/5, 12/5).
Because the extreme value theorem fails to hold (why?), we can only claim that if this
problem has a solution, then it must be (x ∗
1, x∗
2) = (3/5, 2/5).
ECON 2050  Optimization III
27 / 28
```
