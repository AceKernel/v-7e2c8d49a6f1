# Lecture 11: Reduced Lagrangian

PDF page 6 of 25; printed slide 6.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=6) | [Previous](page-lecture-11-05.md) | [Next](page-lecture-11-07.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Alternatively, one can also set up the Lagrangian without considering the nonnegativity
constraints:
˜L(x, λ) = f (x) −λ1g1(x) −λ2g2(x) −· · · −λmgm(x),
and the KKT conditions can be expressed in the following equivalent way: if x ∗≥0 is a
solution to the non-linear program with non-negative variables, then there exists
λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∂˜L(x∗, λ∗)
∂x1
≤0, . . . , ∂˜L(x∗, λ∗)
∂xn
≤0,
(2)
x∗
1
∂˜L(x∗, λ∗)
∂x1
= 0, . . . , x∗
n
∂˜L(x∗, λ∗)
∂xn
= 0,
(3)
∂˜L(x∗, λ∗)
∂λ1
≥0, . . . , ∂˜L(x∗, λ∗)
∂λm
≥0,
(4)
λ∗
1
∂˜L(x∗, λ∗)
∂λ1
= 0, . . . , λ∗
m
∂˜L(x∗, λ∗)
∂λm
= 0.
(5)
ECON 2050  Optimization IV
6 / 25
```
