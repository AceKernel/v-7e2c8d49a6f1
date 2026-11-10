# Lecture 10: Multipliers from linear-programming duality

PDF page 10 of 28; printed slide 10.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=10) | [Previous](page-lecture-10-09.md) | [Next](page-lecture-10-11.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Because the primal has a solution h = 0, which leads to optimal value 0. By the duality
theorem, the optimal value of the dual is also 0, implying that
−λ∗
1g1(x∗) −λ∗
2g2(x∗) −· · · −λ∗
mgm(x∗) = 0.
Because λ∗
i ≥0 and gi(x∗) ≤0, −λ∗
i gi(x∗) ≥0 for all i = 1, . . . , m. Thus, it must be that
λ∗
i gi(x∗) = 0
for all i = 1, . . . , m.
(complementary slackness)
Since the dual constraints must be satised, we see that a set of necessary conditions for x ∗
being a solution of the non-linear program is that there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0,
gi(x∗) ≤0
for all i = 1, . . . , m,
λ∗
i gi(x∗) = 0
for all i = 1, . . . , m.
These conditions are sometimes called the Langrange conditions; the dual variables λ1, . . . ,
λm are also called Lagrange multipliers.
ECON 2050  Optimization III
10 / 28
```
