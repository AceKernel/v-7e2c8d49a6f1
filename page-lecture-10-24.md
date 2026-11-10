# Lecture 10: Unrestricted equality multipliers

PDF page 24 of 28; printed slide 24.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=24) | [Previous](page-lecture-10-23.md) | [Next](page-lecture-10-25.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Thankfully, the power of the duality theorem allows us to handle equality constraints easily.
The linear program on slide 8 now becomes, replacing ≤by =,
max
h
∇f (x∗) · h
subject to
∇gi(x∗) · h = −gi(x∗) for all i = 1, . . . , m.
Its dual is
min
λ −λ1g1(x∗) −λ2g2(x∗) −· · · −λmgm(x∗)
s.t. λ1∇g1(x∗) + λ2∇g2(x∗) + · · · + λm∇gm(x∗) = ∇f (x∗)
The only dierence is that the sign of the dual variables (Lagrange multipliers) are unrestricted.
Because the constraints are equalities rather than inequalities, complementary slackness is
no longer meaningful.
ECON 2050  Optimization III
24 / 28
```
