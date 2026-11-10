# Lecture 7: Convexity of a constraint set

PDF page 25 of 30; printed slide 25.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=25) | [Previous](page-lecture-07-24.md) | [Next](page-lecture-07-26.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: S =
{︁
(x, y, z) ∈R3 : x2 + y2 ≤1, z = 1
}︁
is convex, because
f (x, y) = x2 + y2 is convex (will be proved later);
thus epi(f ) =
{︁
(x, y, z) ∈R3 : z ≥x2 + y2}︁
is convex;
S = intersection of epi(f ) with the plane described by z = 1, which is also convex
Exercise: Prove that the set T =
{︁
(x, y) : y ≥x2}︁
is convex.
We know that g(x) = x2 is a convex function. Since T = epi(g), by the previous proposition,
T is a convex set.
ECON 2050 – Convexity
25 / 30
```
