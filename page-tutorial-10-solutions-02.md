# Tutorial 10 solutions: P1: Affine-constraint Lagrange cases; P2: Equality-circle constraint and existence

PDF page 2 of 7.

[Page map](map-tutorial-10-solutions.md) | [Original PDF page](tutorial-10-solutions.pdf#page=2) | [Previous](page-tutorial-10-solutions-01.md) | [Next](page-tutorial-10-solutions-03.md)

Topics: existence, lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
• λ1 > 0 and λ2 > 0. Complementary slackness imply that we have two equations
and two unknowns: x1 + x2 = 4, x1 + 3x2 = 9; the solution is x1 = 1.5 and
x2 = 2.5. Then the first two equations of the Lagrange conditions become
5 −λ1 −λ2 = 0
3 −λ1 −3λ2 = 0
implying that λ1 = 6 and λ2 = −1, which violates the condition λ2 ≥0.
Thus, the unique point that satisfies the Lagrange conditions is (x∗
1, x∗
2, λ∗
1, λ∗
2) = (2, 2, 4, 0).
Note. We can solve this problem graphically:
x1
x2
(x∗
1, x∗
2) = (2, 2)
x1 + 3x2 = 9
x1 + x2 = 4
0
4
9
Level curves of −(x1 −4)2 −(x2 −4)2
Indeed, the unique solution is (x∗
1, x∗
2) = (2, 2), confirming that every solution must satisfy
the Lagrange conditions.
Problem 2
Consider the maximization problem
max
(x,y)∈R2 x −y
subject to
x2 + y2 = 8
(a) Does a solution to this maximization problem exist? Explain.
(b) Find all solutions to this maximization problem.
Solution:
(a) Since the objective function is linear, it is continuous. Moreover, the constraint set C is
compact because it is the circle centered at the origin with radius 2
√
2. By the extreme
value theorem, a solution exists.
(b) Define the constraint function g : R2 →R by g(x, y) = x2+y2−8. Note that ∇g(x, y) ̸=
(0, 0) for all (x, y) ∈C = {(x, y) ∈R2 :
x2 + y2 = 8} as ∇g(x, y) = (2x, 2y) =
(0, 0) only if (x, y) = (0, 0) /∈C. Thus, {∇g(x, y)} is linearly independent for all
(x, y) ∈C. Therefore, the Lagrange conditions are necessary; i.e., every solution to the
maximization problem must satisfy the Lagrange conditions.
2
```
