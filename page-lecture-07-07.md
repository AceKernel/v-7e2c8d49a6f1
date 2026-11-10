# Lecture 7: Intersections of convex sets

PDF page 7 of 30; printed slide 7.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=7) | [Previous](page-lecture-07-06.md) | [Next](page-lecture-07-08.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Proposition
Every intersection of convex sets is a convex set.
Proof:
Suppose Si for i ∈I, are convex sets (where I is some “index” set, e.g. I = {1, 2, 3}).
If x, y ∈⋂︁
i∈I Si then x, y ∈Si for every i ∈I.
For every i, since Si is convex, the line segment between x and y, [x, y], is contained in
Si.
Therefore, [x, y] belongs to the intersection ⋂︁
i∈I Si.
Example: S =
{︁
(x, y) ∈R2 : x + 2y ≤3, x ≥0, y ≥0
}︁
is convex because
S = T ∩{(x, y) ∈R2 : x ≥0} ∩{(x, y) ∈R2 : y ≥0},
where T =
{︁
(x, y) ∈R2 : x + 2y ≤3
}︁
, and it is not difficult to check that both
{(x, y) ∈R2 : x ≥0}, {(x, y) ∈R2 : y ≥0} are convex (exercises; use definition).
ECON 2050 – Convexity
7 / 30
```
