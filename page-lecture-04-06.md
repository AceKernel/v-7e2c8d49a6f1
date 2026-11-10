# Lecture 4: Chain-rule production exercise

PDF page 6 of 25; printed slide 6.

[Page map](map-lecture-04.md) | [Original PDF page](lecture-04.pdf#page=6) | [Previous](page-lecture-04-05.md) | [Next](page-lecture-04-07.md)

Topics: chain-hessian.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Exercise: Consider the production function Q = 2K 2L. Suppose that the inputs K and L vary
with the interest rate r, via the expressions
K(r) =
1
ln(r + 1),
and
L(r) = 100 + 25r.
What is the rate of change of output Q?
We apply the chain rule:
dQ
dr = ∂Q
∂K · K ′(r) + ∂Q
∂L · L′(r)
= 4K(r)L(r) ·
(︃
−
1
(r + 1)[ln(r + 1)]2
)︃
+ 2K 2(r) · 25
= −
400 + 100r
(r + 1)[ln(r + 1)]3 +
50
[ln(r + 1)]2 .
ECON 2050 – Basic Real Analysis IV
6 / 25
```
