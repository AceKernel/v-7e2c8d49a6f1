# Lecture 7: Unions need not be convex

PDF page 8 of 30; printed slide 8.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=8) | [Previous](page-lecture-07-07.md) | [Next](page-lecture-07-09.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Warning: In general, the union of convex sets is not a convex set.
Exercise: Write down or draw two convex sets S and T whose union S ∪T is not convex.
S = {1} and T = {2} are convex, but S ∪T = {1, 2} is not convex.
S = [1, 2] and T = [3, 4] are convex, but S ∪T = [1, 2] ∪[3, 4] is not convex: x′ = 2 and
x′′ = 3 are contained in S ∪T, but (1/2)x′ + (1/2)x′′ = (1/2)2 + (1/2)3 = 2.5 /∈S ∪T
S = B1(1, 0) and T = B1(−1, 0) are convex but S ∪T is not convex.
(E.g. (1, 1
2) ∈S and (−1, 1
2) ∈T both belong to S ∪T, but the midpoint (0, 1
2) of the
line segment [(1, 1
2), (−1, 1
2)] does not belong to either of the two sets and, therefore, it
does not belong to the union of them.)
ECON 2050 – Convexity
8 / 30
```
