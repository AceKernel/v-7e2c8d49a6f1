# Lecture 10: Quadratic-constraint exercise

PDF page 21 of 28; printed slide 21.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=21) | [Previous](page-lecture-10-20.md) | [Next](page-lecture-10-22.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Exercise: Solve the maximization problem
max
(x,y)∈R2 f (x, y) = x + y
s.t.
g(x, y) = x2 + y2 −2 ≤0.
By the extreme value theorem, the maximization problem has a solution.
Since ∇g(x, y) = (2x, 2y) = (0, 0) only if (x, y) = (0, 0), {∇g(x, y)} is linearly
independent for every (x, y) in the constraint set except for (0, 0).
However, (0, 0) doesn't make the constraint bind, and therefore the set of gradients of the
binding constraints is always linearly independent.
Thus, the Lagrange conditions are necessary; i.e., every solution of this problem must
satisfy the Lagrange conditions.
ECON 2050  Optimization III
21 / 28
```
