# Tutorial 9 solutions: P2: Juice-factory linear program, dual and resource values; P3: A linear program and sensitivity

PDF page 4 of 6.

[Page map](map-tutorial-09-solutions.md) | [Original PDF page](tutorial-09-solutions.pdf#page=4) | [Previous](page-tutorial-09-solutions-03.md) | [Next](page-tutorial-09-solutions-05.md)

Topics: duality, graphs, linear-programming.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
(d) The dual variable 𝑦1 can be interpreted as the marginal value of labor, or more specifi-
cally, the relative contribution that one unit of labor makes to the total revenue. Simi-
larly, 𝑦2 and 𝑦3 are the marginal values of total production capacity and production limit
of orange juice, respectively.
Alternatively, one can also interpret each dual variables as the imputed cost of using an
extra unit of each of the resources.
(e) By the duality theorem, since the primal has a solution by part (a), the optimal value of
the primal and the dual must coincide.
Problem 3
Consider the linear programming problem
max 2𝑥+ 7𝑦
s.t. 4𝑥+ 5𝑦≤20,
3𝑥+ 7𝑦≤21,
𝑥≥0, 𝑦≥0.
(a) Use the fundamental theorem of linear programming to find a solution to the linear
program; you can assume that a solution exists.
(b) Write down the dual of the linear program.
(c) Suppose the solution to the dual is (𝜆1, 𝜆2) = (0, 1). Then if we change 20 to 20.1 and 21 to
20.8. What is the corresponding change in the optimal value of the objective function?
Solution:
(a) The extreme points (or vertices or corners) of the constraint set are (0, 0), (0, 3), (5, 0),
and (
35
13, 24
13) . To find the solution, we evaluate the value of 𝑓(𝑥, 𝑦) ≡2𝑥+ 7𝑦at each of
the extreme points:
𝑓(0, 0) = 0,
𝑓(0, 3) = 21,
𝑓(5, 0) = 10,
𝑓(
35
13, 24
13) = 238
13 .
Since 21 is the largest, a solution is (𝑥∗, 𝑦∗) = (0, 3).
(b) The dual is
min 20𝜇1 + 21𝜇2
s.t. 4𝜇1 + 3𝜇2 ≥2,
5𝜇1 + 7𝜇2 ≥7,
𝜇1 ≥0, 𝜇2 ≥0.
(c) Recall that the dual variable can be interpreted as the per unit increase in objective func-
tion value from relaxing one of the primal constraints for a sufficiently small amount.
Then by changing 20 to 20.1 and 21 to 20.8, the change in the optimal value of the objec-
tive function is
𝜆1(20.1 −20) + 𝜆2(20.8 −21) = 0(0.1) + 1(−0.2) = −0.2.
4
```
