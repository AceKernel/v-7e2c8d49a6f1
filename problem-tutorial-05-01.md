# Tutorial 5, Problem 1: Linear independence and span of vector families

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-05-solutions.md) | [Original PDF](tutorial-05-solutions.pdf)

Topics: linear-algebra.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-05-solutions.pdf#page=1)

```text
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

## PDF page 2

[Original page](tutorial-05-solutions.pdf#page=2)

```text
ECON 2050
S2 2026
For its span,
span(S3) = {a1(0, 1, 0) + a2(−2, 2, 0) : a1, a2 ∈R} = {(−2a2, a1 + 2a2, 0) : a1, a2 ∈R} .
Note that no matter what a1 and a2 we choose, the third entry is always zero. And
any vector (x, y, 0) ∈R2 can be written as (−2a2, a1 + 2a2) by letting a2 = −x/2 and
a1 = y + x. Thus,
span(S3) = {(x, y, 0) : x, y ∈R}.
Geometrically, the set of all vectors where the z-component is zero forms a flat, two-
dimensional plane, sometimes called the xy-plane.
(iv) S4 is linearly dependent because (−2, 3, 0) = (0, 1, 0) + (−2, 2, 0), or equivalently,
(−2, 3, 0) −(0, 1, 0) −(−2, 2, 0) = (0, 0, 0).
By comparing S3 in part (iii) and S4, we see that S4 = S3 ∪{(−2, 3, 0)}. But since the
vector (−2, 3, 0) can be written as a linear combination of elements in S3, it belongs to
the span of S3, and therefore including this vector doesn’t enlarge the span. Therefore,
span(S4) = span(S3) = {(x, y, 0) : x, y ∈R}.
(v) To determine whether S5 is linearly independent, we consider
a1(1, 1, 0) + a2(0, −3, 1) + a3(2, 4, −1) = (0, 0, 0).
This is equivalent to
a1 + 2a3 = 0
a1 −3a2 + 4a3 = 0
a2 −a3 = 0
We see from the last equation that a2 = a3; plugging it to the second equation, we get
a1 + a3 = 0. Now compare it with the first equation, we get a3 = 0. Then because
a2 = a3 and a1 + a3 = 0, it must be that a1 = a2 = a3 = 0, showing that S5 is linearly
independent.
It is routine to see that
span(S5) = {a1(1, 1, 0) + a2(0, −3, 1) + a3(2, 4, −1) : a1, a2, a3 ∈R}
= {(a1 + 2a3, a1 −3a2 + 4a3, a2 −a3) : a1, a2, a3 ∈R}.
One can verify that every vector (x1, x2, x3) ∈R3 can be written as (a1 + 2a3, a1 −
3a2 + 4a3, a2 −a3) by solving the system of equations
a1 + 2a3 = x1
a1 −3a2 + 4a3 = x2
a2 −a3 = x3
and getting
a1 = −x1 + 2x2 + 6x3
a2 = x1 −x2 −2x3
a2 = x1 −x2 −3x3
Thus, span(S5) = R3.
2
```

## PDF page 3

[Original page](tutorial-05-solutions.pdf#page=3)

```text
ECON 2050
S2 2026
```
