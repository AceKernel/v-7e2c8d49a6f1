# Lecture 11: Disk-constraint exercise

PDF page 12 of 25; printed slide 12.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=12) | [Previous](page-lecture-11-11.md) | [Next](page-lecture-11-13.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Exercise: Consider the maximization problem
max f (x, y) = x + y
s.t.
x2 + y2 ≤2, x ≥0, y ≥0
Denote the three constraint functions by g(x, y) = x 2 + y2 −2, n1(x, y) = −x,
n2(x, y) = −y.
The linear independence condition is satised at all relevant points:
▶If exactly 1 constraint binds, the corresponding gradient is non-zero:
⋆If x = 0 is the only binding constraint, since ∇n1(x, y) = (−1, 0), the set of gradients of binding
constraint functions is {(−1, 0)}, which is linearly independent.
⋆If y = 0 is the only binding constraint, since ∇n2(x, y) = (0, −1), the set of gradients of binding
constraint functions is {(0, −1)}, which is linearly independent.
⋆If x2 + y 2 = 2 is the binding constraint, since ∇g(x, y) = (2x, 2y), it is only zero when
(x, y) = (0, 0), but the constraint doesn't bind at this point. Thus, {∇g(x, y)} is linearly
independent when g(x, y) ≤0 is binding.
ECON 2050  Optimization IV
12 / 25
```
