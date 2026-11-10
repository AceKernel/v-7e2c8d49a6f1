# Tutorial 7, Problem 4: Convexity and concavity by composition

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-07-solutions.md) | [Original PDF](tutorial-07-solutions.pdf)

Topics: convexity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 3

[Original page](tutorial-07-solutions.pdf#page=3)

```text
Problem 4
Analyze whether the following functions are concave or convex.
1. f1(x, y) = 4x2 + e2y2.
2. f2(x, y) = ln(3x + 2y).
Solution:
1. Observe that f1(x, y) = g1(x) + h1(y), where g1(x) = 4x2, and h1(y) = e2y2. Now
g1(x) is convex, and h1(y) = m ◦n, where m(u) = eu is increasing and convex, and
n(y) = 2y2 is convex. Thus, both g1 and h1 are convex; by the result we proved in
Problem 2, f1(x, y) is also convex.
2. f2(x, y) = ln(3x + 2y) is concave because f2 = h2 ◦g2, where h2(u) = ln u is an
increasing concave function, and g2(x, y) = 3x + 2y is linear and hence concave.
```
