# Lecture 11: Logarithmic example

PDF page 10 of 25; printed slide 10.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=10) | [Previous](page-lecture-11-09.md) | [Next](page-lecture-11-11.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: Consider the maximization problem
max
(x1,x2)∈R2
x1x2
s.t.
x1 + x2 ≤6
x1 ≥0,
x2 ≥0.
Observe that the constraint functions are ane, so the KKT conditions are necessary; that
is, every solution of the maximization problem must satisfy the KKT conditions.
The KKT conditions are
x2 −λ ≤0,
x1(x2 −λ) = 0,
x1 ≥0,
x1 −λ ≤0,
x2(x1 −λ) = 0,
x2 ≥0,
x1 + x2 −6 ≤0,
λ(x1 + x2 −6) = 0,
λ ≥0.
If x1 > 0, since x1(x2 −λ) = 0, we must have x2 = λ. If x2 = λ = 0, then x1 −λ ≤0
implies that x1 ≤0, a contradiction. Thus, x2 > 0.
But then x2(x1 −λ) = 0 implies that x1 = λ = x2 > 0.
ECON 2050  Optimization IV
10 / 25
```
