# Lecture 5: Row-combination interpretation

PDF page 23 of 26; printed slide 23.

[Page map](map-lecture-05.md) | [Original PDF page](lecture-05.pdf#page=23) | [Previous](page-lecture-05-22.md) | [Next](page-lecture-05-24.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Algebraic intuition:
Take any linear combination of the equations in the system Ax = b.
This linear combination can be obtained by multiplying each side of the system by a
suitable vector y: yAx = y · b.
Any vector that solves the first system must also solve the second.
If yA = 0, then yAx = 0 · x = 0 for any x ∈Rn. But then y · b ̸= 0 implies that
yAx ̸= y · b.
Thus, there doesn’t exists a vector x such that yAx ̸= y · b, which in turn implies that
Ax = b is impossible.
ECON 2050 – Linear Algebra I
23 / 26
```
