# Tutorial 8 solutions: P2: Logarithmic domain and absence of extrema; P3: Existence on a disk and a triangle

PDF page 3 of 5.

[Page map](map-tutorial-08-solutions.md) | [Original PDF page](tutorial-08-solutions.pdf#page=3) | [Previous](page-tutorial-08-solutions-02.md) | [Next](page-tutorial-08-solutions-04.md)

Topics: continuity, existence, graphs, unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
x
y
Shaded region: C
(equivalent to {(x, y) ∈R2 : y > (x−2)2
8
−1
2})
Black dashed curve: boundary
(8y −x2 + 4x = 0, not contained in C)
Problem 3
Use extreme value theorem to show that the following maximization problems have a
solution.
(a) max(x,y)∈C f(x, y), where f(x, y) = 2xy2, and
C = {(x, y) ∈R2 : x2 + y2 ≤1}.
(b) max(x,y)∈D g(x, y), where g(x, y) = 4x + 7y, and
D = {(x, y) ∈R2 : x + 2y ≤3, x ≥0, y ≥0}.
Solution:
(a) Observe that f = 2(pr1)(pr2)(pr2). Since the projections pr1 and pr2 are continuous,
so is their product; moreover, multiplying a function by 2 doesn’t change it continuity.
Thus, the objective function f is continuous.
The set C is closed because it contains all its boundary points (every point in the set
{(x, y) ∈R2 : x2 + y2 = 1} is a boundary point, which is contained in C), and it is also
bounded because for all (x, y) ∈C, ∥(x, y)∥≤1. Therefore, C is compact.
Then by the extreme value theorem, the maximization problem max(x,y)∈C f(x, y) has a
solution.
Graphically, C is the closed ball centered at (0, 0) with radius 1; its boundary is the circle
in black.
x
y
O
(1, 0)
(−1, 0)
(0, 1)
(0, −1)
r = 1
3
```
