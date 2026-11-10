# Tutorial 5 solutions: P4: Linear-system feasibility and certificates

PDF page 5 of 5.

[Page map](map-tutorial-05-solutions.md) | [Original PDF page](tutorial-05-solutions.pdf#page=5) | [Previous](page-tutorial-05-solutions-04.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
(1) Determine whether the system has a solution.
(2) (Extra Practice Problem) Determine whether the system has a solution, and if a
solution exists, whether it has one or infinitely many solutions.
Solution:
(1) Take any vector y = (y1, y2), and let
yA =
y1
y2
 
4
1
−2
1
0
5

=
4y1 + y2
y1
−2y1 + 5y2

=
0
0
0
.
Then it must be that y1 = 0, and plugging this into 4y1 + y2 = 0, we have y2 = 0.
Consequently, y · b = 0 · −2 + 0 · 3 = 0. Thus, whenever yA = 0, it must be that
y · b = 0. The theorem on the slides then indicates that the system has a solution.
(2) We have
[A|b] =

4
1
−2
−2
1
0
5
3

;
it is routine to verify that rank(A) = rank([A|b]) = 2 < 3 = n, and therefore by the
theorem on the slides, the system of equations has infinitely many solutions.
5
```
