# Tutorial 9 solutions: P2: Juice-factory linear program, dual and resource values

PDF page 3 of 6.

[Page map](map-tutorial-09-solutions.md) | [Original PDF page](tutorial-09-solutions.pdf#page=3) | [Previous](page-tutorial-09-solutions-02.md) | [Next](page-tutorial-09-solutions-04.md)

Topics: duality, graphs, linear-programming.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
(a) Use the extreme value theorem to determine whether the problem has a solution.
(b) Use the fundamental theorem of linear programming to find a solution to the linear
program.
(c) Write down the dual of this linear program.
(d) Interpret the dual variables.
(e) Determine whether the optimal value of the dual is the same as the primal above.
Solution:
(a) Because the objective function is linear, it is continuous. The constraint set 𝐷, shaded in
orange in the picture below, is a compact set. Then by the extreme value theorem, the
linear programming problem has a solution.
𝑥1
𝑥2
𝑥1 + 8
3𝑥2 = 4
𝑥1 + 𝑥2 = 2
𝑥1 = 3
2
(0, 0)
(3
2, 0)
( 3
2, 1
2)
( 4
5, 6
5)
(0, 3
2)
𝐷
(b) By the fundamental theorem of linear programming, since a solution exists by part (a),
an extreme point (or vertex or corner) of the constraint set must be a solution. Therefore,
it suffices to compare the value of the objective function 𝑓(𝑥1, 𝑥2) ≡𝑥1 + 2𝑥2 at the five
extreme points: (0, 0), (0, 3/2), (4/5, 6/5), (3/2, 1/2), (3/2, 0). Now
𝑓(0, 0) = 0, 𝑓(0, 3/2) = 3, 𝑓(4/5, 6/5) = 16/5, 𝑓(3/2, 1/2) = 5/2, 𝑓(3/2, 0) = 3/2.
Since 16/5 is the largest, a solution of this linear programming problem is (𝑥∗
1, 𝑥∗
2) =
(4/5, 6/5).
(c) The dual is
min 4𝑦1 + 2𝑦2 + 3
2𝑦3
s.t. 𝑦1 + 𝑦2 + 𝑦3 ≥1,
8
3𝑦1 + 𝑦2 ≥2,
𝑦1 ≥0, 𝑦2 ≥0, 𝑦3 ≥0.
3
```
