# Lecture 3: Testing total differentiability

PDF page 27 of 31; printed slide 27.

[Page map](map-lecture-03.md) | [Original PDF page](lecture-03.pdf#page=27) | [Previous](page-lecture-03-26.md) | [Next](page-lecture-03-28.md)

Topics: differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
If it exists, the derivative of f at (0, 0) is given by (a1, a2) such that:
lim
n→∞
|f (x1n, x2n) −f (0, 0) −a1x1n −a2x2n|
√︂
x2
1n + x2
2n
= 0
or,
lim
n→∞
⃓⃓⃓⃓⃓
x2
1x2
x2
1n + x2
2n
−a1x1n −a2x2n
⃓⃓⃓⃓⃓·
1
√︂
x2
1n + x2
2n
= 0
1. Take the sequence (x1n, x2n) =
(︁1
n, 1
n
)︁
. Then the above limit becomes:
lim
n→∞
⃓⃓⃓⃓⃓
1
n3
2
n2
−a1
n −a2
n
⃓⃓⃓⃓⃓
1
√
2
n
= lim
n→∞
⃓⃓⃓⃓
1
2
√
2
−a1 + a2
√
2
⃓⃓⃓⃓= 0
which is satisfied if and only if
a1 + a2 = 1
2
(1)
ECON 2050 – Basic Real Analysis III
27 / 31
```
