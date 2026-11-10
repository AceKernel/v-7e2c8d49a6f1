# Tutorial 6 solutions: P1: Cones, sub-cones and nonnegative feasibility; P2: A Farkas feasibility certificate; P3: Deriving inequality alternatives

PDF page 2 of 4.

[Page map](map-tutorial-06-solutions.md) | [Original PDF page](tutorial-06-solutions.pdf#page=2) | [Previous](page-tutorial-06-solutions-01.md) | [Next](page-tutorial-06-solutions-03.md)

Topics: farkas, graphs.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
y1
y2
O
2y1 + y2 = 0
y2 = 0
y1 = 0
y1 = 2y2
2y1 + y2 ≥0
y2 ≥0
y1 ≤2y2
y1 < 0
Problem 2
Use the Farkas lemma to decide if the following system has a non-negative solution:

4
1
−5
1
0
2
 

x1
x2
x3

=

1
1

.
Solution: The Farkas alternative is
y1
y2
 
4
1
−5
1
0
2

≥
0
0
0
,
and
y1 + y2 < 0.
As a system of inequalities the alternative is:
4y1 + y2 ≥0,
y1 + 0y2 ≥0,
−5y1 + 2y2 ≥0,
y1 + y2 < 0.
There can be no solution to this system. The second inequality requires that y1 ≥0. Combin-
ing this with the last inequality we conclude that y2 < 0. But y1 ≥0 and y2 < 0 contradict
−5y1 + 2y2 ≥0. Thus, the original system has a non-negative solution.
Problem 3
Let A be a m×n matrix, and let b ∈Rm. Prove, using the Farkas Lemma, the following:
(1) Either the system Ax ≥b has a non-negative solution, or there is a non-negative
y ∈Rm such that yA ≤0 and y · b > 0, but not both.
(2) (Extra Practice Problem) Either the system Ax ≤b has a solution, or there is a
non-negative y ∈Rm such that yA = 0 and y · b < 0, but not both.
(Hint. Recall how we found the Farkas alternative for the system Ax ≤b and x ≥0 in the
lecture.)
Solution:
2
```
