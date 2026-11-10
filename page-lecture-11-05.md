# Lecture 11: Reduced KKT conditions

PDF page 5 of 25; printed slide 5.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=5) | [Previous](page-lecture-11-04.md) | [Next](page-lecture-11-06.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Karush-Kuhn-Tucker (KKT) conditions
Going back to the more general maximization problem (♢), we see that a set of necessary
conditions for x∗≥0 being a solution to the non-linear program with non-negative variables is
that there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) ≤0,
x∗
i
(︃∂f (x∗)
∂xi
−λ∗
1
∂g1(x∗)
∂xi
−λ∗
2
∂g2(x∗)
∂xi
−· · · −λ∗
m
∂gm(x∗)
∂xi
)︃
= 0
for all i = 1, . . . , n,
gj(x∗) ≤0
for all j = 1, . . . , m,
λ∗
j gj(x∗) = 0
for all j = 1, . . . , m.
These conditions are sometimes called the Karush-Kuhn-Tucker (KKT) conditions.
ECON 2050  Optimization IV
5 / 25
```
