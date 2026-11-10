# Lecture 1: Proof of the sum rule

PDF page 23 of 30; printed slide 23.

[Page map](map-lecture-01.md) | [Original PDF page](lecture-01.pdf#page=23) | [Previous](page-lecture-01-22.md) | [Next](page-lecture-01-24.md)

Topics: sequences.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Proof of part (a): Let ε > 0.
1 Since xn →x∗, ∃N1 ∈N such that ∥xn −x∗∥< ε/2 for all n ≥N1.
2 Since yn →y ∗, ∃N2 ∈N such that ∥yn −y ∗∥< ε/2 for all n ≥N2.
Therefore ∥xn −x∗∥< ε/2 and ∥yn −y ∗∥< ε/2 for all n ≥N ≡max{N1, N2}. Then for all
n ≥N,
∥(xn + yn)−(x∗+ y ∗)∥= ∥(xn −x∗) −(y ∗−yn)∥
≤∥(xn −x∗) −0∥+ ∥0 −(y ∗−yn)∥(by triangle inequality)
= ∥xn −x∗∥+ ∥yn −y ∗∥
< ε
2 + ε
2
= ε,
where 0 = (0, . . . , 0). Thus, (xn + yn) →(x∗+ y ∗).
ECON 2050 – Basic Real Analysis I
23 / 30
```
