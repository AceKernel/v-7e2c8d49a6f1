# Lecture 1: Convergence and present value

PDF page 10 of 30; printed slide 10.

[Page map](map-lecture-01.md) | [Original PDF page](lecture-01.pdf#page=10) | [Previous](page-lecture-01-09.md) | [Next](page-lecture-01-11.md)

Topics: sequences.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Often, we want to figure out where a sequence “tends to” as the index n ∈N becomes “large”
(i.e., goes to +∞)
Example: Interest rate = 3.5% (both for saving and borrowing). Your bank offers to pay you
(and your offspring) $1000/year for n years. How much should you maximally pay for this?
If n = 1, then the maximum you should pay is:
PV1 = 1000
If n = 2, then the maximum you should pay is:
PV2 = 1000 + 1000
1.035 ≈1000 + 966 = 1966
More generally,
PVn = 1000 + 1000
1.0351 + . . . +
1000
1.035n−1
=
n−1
∑︂
k=0
1000
1.035k = 1000 ·
k−1
∑︂
k=0
(︃
1
1.035
)︃k
ECON 2050 – Basic Real Analysis I
10 / 30
```
