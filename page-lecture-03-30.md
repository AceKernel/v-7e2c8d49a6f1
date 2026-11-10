# Lecture 3: Existing partial derivatives without differentiability

PDF page 30 of 31; printed slide 30.

[Page map](map-lecture-03.md) | [Original PDF page](lecture-03.pdf#page=30) | [Previous](page-lecture-03-29.md) | [Next](page-lecture-03-31.md)

Topics: differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
We now check that all partial derivatives exist. Recall the definition of partial derivative with
respect to x1 at x0:
lim
n→∞
f (x10 + hn, x20) −f (x10, x20)
hn
.
For x0 = (0, 0), this simplifies to
lim
n→∞
f (hn, 0) −f (0, 0)
hn
;
and the given f this becomes (recalling that the sequence (hn) is such that hn →0 and hn ̸= 0
for all n)
lim
n→∞
(hn)2·0
(hn)2+02 −0
hn
= 0.
An analogous argument shows that the definition of partial derivative with respect to x2 at x0
also exists and equals zero.
ECON 2050 – Basic Real Analysis III
30 / 31
```
