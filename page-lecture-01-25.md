# Lecture 1: Coordinatewise convergence

PDF page 25 of 30; printed slide 25.

[Page map](map-lecture-01.md) | [Original PDF page](lecture-01.pdf#page=25) | [Previous](page-lecture-01-24.md) | [Next](page-lecture-01-26.md)

Topics: sequences.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem (compare SB Thm 12.5)
Let (xn)n∈N be a sequence with codomain Rm. Then
lim
n→∞xn = x∗
if and only if
(︂
lim
n→∞xi,n = x∗
i for all i = 1, . . . , m
)︂
.
We can use this theorem to verify that “Ann converges to (0, 0)”:
We have
lim
t→∞x1,t = lim
t→∞
30
t sin
(︃30
t
)︃
= 0
We have
lim
t→∞x2,t = lim
t→∞
30
t cos
(︃30
t
)︃
= 0
Therefore,
lim
t→∞xt =
(︃30
t sin
(︃30
t
)︃
, 30
t cos
(︃30
t
)︃)︃
= (0, 0)
ECON 2050 – Basic Real Analysis I
25 / 30
```
