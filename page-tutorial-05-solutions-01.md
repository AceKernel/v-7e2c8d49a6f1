# Tutorial 5 solutions: P1: Linear independence and span of vector families

PDF page 1 of 5.

[Page map](map-tutorial-05-solutions.md) | [Original PDF page](tutorial-05-solutions.pdf#page=1) | [Next](page-tutorial-05-solutions-02.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Tutorial 5 Solution
Problem 1
Consider the following sets of vectors. Determine (a) whether they are linear indepen-
dent or linearly dependent, and (b) their spans.
(i) S1 = {(1, −2), (2, −4)};
(ii) S2 = {(1, 0), (0, 1)};
(iii) S3 = {(0, 1, 0), (−2, 2, 0)};
(iv) S4 = {(0, 1, 0), (−2, 2, 0), (−2, 3, 0)};
(v) S5 = {(1, 1, 0), (0, −3, 1), (2, 4, −1)}.
Solution:
(i) We know from lecture slides that S1 is linearly dependent; and
span(S1) = {a1(1, −2) + a2(2, −4) : a1, a2 ∈R} .
Since (2, −4) = 2(1, −2), we can simplify it to
span(S1) = {a1(1, −2) + 2a2(1, −2) : a1, a2 ∈R} = {(a1 + 2a2)(1, −2) : a1, a2 ∈R} .
If we let k = c1 +2c2, we can see that any vector in the span is just a scalar multiple of
(1, −2). This is precisely the line that passes through the origin and the point (1, −2).
In other words, the span is the set of all points (x, y) that satisfy the equation y = −2x.
(ii) To see that whether S2 is linearly independent, consider
a1(1, 0) + a2(0, 1) = (0, 0).
This is equivalent to a1 = 0 and a2 = 0, and therefore S2 must be linearly independent.
And its span is given by
span(S2) = {a1(1, 0) + a2(0, 1) : a1, a2 ∈R} = {(a1, a2) : a1, a2 ∈R} = R2.
(iii) Again, we consider the equality
a1(0, 1, 0) + a2(−2, 2, 0) = (0, 0, 0).
Since the left-hand side is equivalent to (−2a2, a1+2a2, 0), the equality above is equiv-
alent to −2a2 = 0 and a1 + 2a2 = 0. Then it must be that a1 = a2 = 0, showing that
S3 is linearly independent.
1
```
