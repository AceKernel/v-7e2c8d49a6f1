# Lecture 9: Fundamental theorem of linear programming

PDF page 9 of 26; printed slide 9.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=9) | [Previous](page-lecture-09-08.md) | [Next](page-lecture-09-10.md)

Topics: linear-programming.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Fundamental theorem of linear programming
First, we formalize the observation suggested by the example: A maximum is an extreme point.
Theorem (Fundamental Theorem of Linear Programming)
Suppose the linear program max{c · x : Ax ≤b, x ≥0} has a solution. Then an extreme point
of the constraint set is a solution.
Example: Revisiting the example from the beginning:
Observe that the constraint set is compact, and therefore a solution exists.
By the fundamental theorem of linear programming, it suces to search within the set of
extreme points of the constraint set D.
The extreme points are (0, 0), (0, 4
3), (2, 0), and (1, 1), and
f (0, 0) = 0,
f
(︃
0, 4
3
)︃
= 8
3,
f (2, 0) = 2,
and
f (1, 1) = 3.
Thus, (1, 1) is a solution.
ECON 2050  Optimization II
9 / 26
```
