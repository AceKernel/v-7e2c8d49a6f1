# Lecture 1: Present-value sequence example

PDF page 11 of 30; printed slide 11.

[Page map](map-lecture-01.md) | [Original PDF page](lecture-01.pdf#page=11) | [Previous](page-lecture-01-10.md) | [Next](page-lecture-01-12.md)

Topics: sequences.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
This defines a sequence (PVn)∞
n=1; up to rounding:
(PVn)∞
n=1 = (1000, 1966, 2900, 3802, 4673, . . .)
Where does (PVn)∞
n=1 “tend to” as n →∞?
PVn = 1000
+ 1000
1.0351 + . . . . . .+
1000
1.035n−2 +
1000
1.035n−1
(1)
1
1.035PVn = 1000
1.0351 + 1000
1.0352 + . . . . . .+
1000
1.035n−1 + 1000
1.035n
(2)
(1) −(2) :
(︃
1 −
1
1.035
)︃
PVn = 1000 −1000
1.035n .
Therefore:
PVn = 1000 −
1000
1.035n
1 −
1
1.035
≈29571 −
1000
1.035n
1 −
1
1.035
(≈29571 for n large)
ECON 2050 – Basic Real Analysis I
11 / 30
```
