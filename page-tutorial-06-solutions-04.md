# Tutorial 6 solutions: P3: Deriving inequality alternatives; P4: A mixed-inequality alternative

PDF page 4 of 4.

[Page map](map-tutorial-06-solutions.md) | [Original PDF page](tutorial-06-solutions.pdf#page=4) | [Previous](page-tutorial-06-solutions-03.md)

Topics: farkas.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Problem 4
Consider the system of equations
x1 + 2x2 + 3x3 ≤5,
x1 + 3x2 −2x3 ≥7,
x1 + x2 + x3 ≤2,
x1 −2x2 −3x3 ≥3,
x1 ≥0,
x2 ≥0,
x3 ≥0.
Write down its Farkas alternative.
(Hint. Try to write down this system in matrix form first. How are you going to deal with
the first four inequalities in doing that?)
Solution: The second and the fourth inequality can be written as
−x1 −3x2 + 2x3 ≤−7
and
−x1 + 2x2 + 3x3 ≤−3,
respectively. Therefore, the system can be written as




1
2
3
−1
−3
2
1
1
1
−1
2
3






x1
x2
x3

≤




5
−7
2
−3




and


x1
x2
x3

≥


0
0
0

.
The system can be written as Ax ≤b and x ≥0; according to our discussions on inequality
systems in the lecture, the Farkas alternative takes the form of yA ≥0, y ≥0, and y·b < 0.
Thus, the Farkas alternative is
y1
y2
y3
y4





1
2
3
−1
−3
2
1
1
1
−1
2
3



≥
0
0
0
,
y1
y2
y3
y4

≥
0
0
0
0
,
and 5y1 −7y2 + 2y3 −3y4 < 0.
4
```
