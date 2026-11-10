# Lecture 10: Lagrangian stationarity

PDF page 26 of 28; printed slide 26.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=26) | [Previous](page-lecture-10-25.md) | [Next](page-lecture-10-27.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
When the constraints are equalities, there is an even closer analogy between the rst-order
conditions and the Lagrange conditions. To see this, consider again the Lagrangian:
L(x, λ) = f (x) −λ1g1(x) −λ2g2(x) −· · · −λmgm(x).
If x∗∈S is a solution to the non-linear program with equality constraints, there exists
λ∗∈Rm:
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
= 0,
∂L(x∗, λ∗)
∂λ1
= g1(x∗) = 0,
· · · ,
∂L(x∗, λ∗)
∂λm
= gm(x∗) = 0.
Therefore, if x∗is a solution, (x∗, λ∗) is a critical point of L(x, λ), where the rst-order
conditions hold.
ECON 2050  Optimization III
26 / 28
```
