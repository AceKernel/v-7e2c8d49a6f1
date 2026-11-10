# Lecture 10: Failure without a qualification

PDF page 14 of 28; printed slide 14.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=14) | [Previous](page-lecture-10-13.md) | [Next](page-lecture-10-15.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The condition ∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0 can also be
obtained through an auxiliary function called the Lagrangian:
L(x, λ) = f (x) −λ1g1(x) −λ2g2(x) −· · · −λmgm(x).
If x∗∈S is a solution to the non-linear program, then there exists a λ∗≥0 such that
∂L(x∗, λ∗)
∂x1
= ∂f (x∗)
∂x1
−λ∗
1
∂g1(x∗)
∂x1
−· · · −λ∗
m
∂gm(x∗)
∂x1
= 0,
∂L(x∗, λ∗)
∂x2
= ∂f (x∗)
∂x2
−λ∗
1
∂g1(x∗)
∂x2
−· · · −λ∗
m
∂gm(x∗)
∂x2
= 0,
...
∂L(x∗, λ∗)
∂xn
= ∂f (x∗)
∂xn
−λ∗
1
∂g1(x∗)
∂xn
−· · · −λ∗
m
∂gm(x∗)
∂xn
= 0.
Therefore, the solution x∗can be interpreted as a critical point of L(x, λ∗), where the
rst-order conditions hold (but don't forget the constraints themselves, gi(x∗) ≤0, and
complementary slackness, λ∗
i gi(x∗) = 0).
ECON 2050  Optimization III
14 / 28
```
