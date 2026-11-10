# Tutorial 7, Problem 6: Intersections of convex sets: extra practice

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-07-solutions.md) | [Original PDF](tutorial-07-solutions.pdf)

Topics: convexity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 4

[Original page](tutorial-07-solutions.pdf#page=4)

```text
Problem 6 (Extra Practice Problem)
Apply the result from Problem 1 and the properties of a convex set to demonstrate that
the following sets are convex.
1. S = {(x, y) ∈R2 : y ≥x2, x2 + y2 ≤4, x ≥0, y ≥0}
2. T = {(x, y) ∈R2 : x2 + y2 ≤25, x + y ≥5, y ≥2, x ≥0}
Solution: (Sketch only)
1. S is convex, as it is the intersection of the following sets, all of which are convex:
• S1 = {(x, y) ∈R2 : y ≥x2} (we showed in Problem 3 that it is convex),
• S2 = {(x, y) ∈R2 : y2 + x2 ≤4} (we showed in Problem 3 that it is convex),
• S3 = {(x, y) ∈R2 : −x ≤0} (convex by Problem 1 because f3(x, y) = −x is
affine and thus convex)
• S4 = {(x, y) ∈R2 : −y ≤0} (convex by Problem 1 because f4(x, y) = −y is
affine and thus convex)
Graphically:
4
```

## PDF page 5

[Original page](tutorial-07-solutions.pdf#page=5)

```text
ECON 2050
S2 2026
2. T is convex, as it is the intersection of the following sets, all of which are convex:
• T1 = {(x, y) ∈R2 : y2 + x2 ≤25} (convex by Problem 1 because g1(x, y) =
x2 + y2 is convex, as we proved in lecture 7),
• T2 = {(x, y) ∈R2 : y ≥5 −x} (convex because T2 = epi(g2), where g2(x) =
5 −x is affine and thus convex),
• T3 = {(x, y) ∈R2 : −x ≤0} (convex by Problem 1 because f3(x, y) = −x is
affine and thus convex)
• T4 = {(x, y) ∈R2 : −y ≤−2} (convex by Problem 1 because f4(x, y) = −y is
affine and thus convex)
Graphically:
5
```
