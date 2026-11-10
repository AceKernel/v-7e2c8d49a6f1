# Lecture 1: Vector convergence and open balls

PDF page 18 of 30; printed slide 18.

[Page map](map-lecture-01.md) | [Original PDF page](lecture-01.pdf#page=18) | [Previous](page-lecture-01-17.md) | [Next](page-lecture-01-19.md)

Topics: sequences, topology.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Definition
Let (xn)n∈N be a sequence with codomain Rm. We say that (xn) converges to x∗or that x∗
is the limit of (xn)n∈N, and write limn→∞xn = x∗or xn →x∗, if
∀ε > 0 ∃N ∈N s.t. ∀n ≥N : ∥xn −x∗∥< ε.
If (xn)n∈N does not converge to any x∗∈Rm we say that (xn)n∈N diverges.
We can rewrite this definition using the notion of open balls:
Definition
The open ball Br(x) with radius r > 0 and center x ∈Rm is the set of points y ∈Rm with
distance less than r from x,
Br(x) = {y ∈Rm : ∥y −x∥< r} .
A sequence (xn)n∈N with codomain Rm converges to x∗if and only if
∀ε > 0 ∃N ∈N s.t. ∀n ≥N : xn ∈Bε(x∗).
ECON 2050 – Basic Real Analysis I
18 / 30
```
