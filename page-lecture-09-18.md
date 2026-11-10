# Lecture 9: Resources and fixed-capacity constraints

PDF page 18 of 26; printed slide 18.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=18) | [Previous](page-lecture-09-17.md) | [Next](page-lecture-09-19.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Consider the example of a bakery on slide 3, with an extra twist that since cakes need to be
refrigerated, there is an extra storage constraint that the at most 6/5 boxes of cakes can be
produced in a day. Thus, the linear program becomes
max
x1 + 2x2
s.t.
x1 + 3x2 ≤4,
x1 + x2 ≤2,
x2 ≤6
5,
x1, x2 ≥0.
It can be veried that the unique optimal solution is still (x ∗
1, x∗
2) = (1, 1).
x1
x2
1
2
3
4
0.5
1
1.5
2
x1 + 3x2 = 4
x1 + x2 = 2
x2 = 6
5
D
(1, 1)
ECON 2050  Optimization II
18 / 26
```
