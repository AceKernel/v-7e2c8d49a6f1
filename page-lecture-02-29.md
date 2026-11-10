# Lecture 2: Definition of differentiability

PDF page 29 of 33; printed slide 29.

[Page map](map-lecture-02.md) | [Original PDF page](lecture-02.pdf#page=29) | [Previous](page-lecture-02-28.md) | [Next](page-lecture-02-30.md)

Topics: differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The formal definition of differentiability is as follows:
Definition
Let D ⊆R be open. The function f : D →R is differentiable at x0 ∈D if there exists
f ′(x0) ∈R such that
f ′(x0) = lim
n→∞
f (x0 + hn) −f (x0)
hn
for all sequences (hn) with hn →0 and hn ̸= 0 for all n. In this case, f ′(x0) is called the
derivative of f at x0.
It is useful to rephrase this definition a bit:
f : D →R is differentiable at x0 if and only if there exists a ∈R such that
lim
n→∞
f (x0 + hn) −f (x0) −ahn
hn
= 0
for all sequences (hn) with hn →0 and hn ̸= 0 for all n. In this case, a = f ′(x0).
ECON 2050 – Basic Real Analysis II
29 / 33
```
