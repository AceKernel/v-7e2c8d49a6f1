# Lecture 2: Equivalent differentiability limit

PDF page 30 of 33; printed slide 30.

[Page map](map-lecture-02.md) | [Original PDF page](lecture-02.pdf#page=30) | [Previous](page-lecture-02-29.md) | [Next](page-lecture-02-31.md)

Topics: differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
f : D →R is differentiable at x0 if and only if there exists a ∈R such that
lim
n→∞
f (xn) −f (x0) −a(xn −x0)
xn −x0
= 0
for all sequences (xn) with xn →x0 and xn ̸= x0 for all n. In this case, a = f ′(x0).
If f : D →R is differentiable at x0, then the tangent line of f at x0, given by
g : R →R, x ↦→f (x0) + f ′(x0)(x −x0)
is an affine function that approximates f around x0 in the sense that whenever |x −x0| is
sufficiently small, the “approximation error” |f (x) −g(x)| is negligible.
ECON 2050 – Basic Real Analysis II
30 / 33
```
