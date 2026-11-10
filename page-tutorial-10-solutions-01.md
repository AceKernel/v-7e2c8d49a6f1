# Tutorial 10 solutions: P1: Affine-constraint Lagrange cases

PDF page 1 of 7.

[Page map](map-tutorial-10-solutions.md) | [Original PDF page](tutorial-10-solutions.pdf#page=1) | [Next](page-tutorial-10-solutions-02.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Tutorial 10 Solution
Problem 1
Consider the maximization problem
max
(x,y)∈R2 −(x1 −4)2 −(x2 −4)2
subject to
x1 + x2 ≤4
and
x1 + 3x2 ≤9.
(a) Are the Lagrange conditions necessary? That is, is it true that every solution of the
maximization problem, if exists, must satisfy the Lagrange conditions?
(b) Write down the Lagrange conditions for this problem.
(c) Find all points that satisfy the Lagrange conditions.
Solution:
(a) The Lagrange conditions are necessary because all constraint functions are affine.
(b) The Lagrange conditions are
−2 (x1 −4) −λ1 −λ2 = 0
−2 (x2 −4) −λ1 −3λ2 = 0
x1 + x2 ≤4, λ1 ≥0, and λ1 (x1 + x2 −4) = 0
x1 + 3x2 ≤9, λ2 ≥0, and λ2 (x1 + 3x2 −9) = 0
(c) We start from the two complementary slackness conditions, λ1 (x1 + x2 −4) = 0 and
λ2 (x1 + 3x2 −9) = 0, by discussing the signs of λ1 and λ2. There are four cases:
• λ1 = λ2 = 0. In this case, the first two equations of the Lagrange conditions above
indicate that x1 = x2 = 4, but this violates the constraint x1+x2 ≤4, and therefore
can’t be the case.
• λ1 > 0 and λ2 = 0. In this case, the first two equations of the Lagrange conditions
above indicate that
x1 = x2 = 4 −λ1/2.
Because λ1 > 0, complementary slackness implies that x1 +x2 = 4. Plugging x1 =
x2 in, we get x1 = x2 = 2, which also satisfies x1+3x2 ≤9. Thus, (x∗
1, x∗
2, λ∗
1, λ∗
2) =
(2, 2, 4, 0) satisfies the Lagrange conditions.
• λ1 = 0 and λ2 > 0. In this case, the first line of the Lagrange conditions can be
written as λ2 = −2(x1 −4); plug into the second line, we get
−2(x2 −4) + 6(x1 −4) = 0
⇔
3x1 −x2 = 8.
Now we have two equations and two unknowns: 3x1 −x2 = 8, x1 + 3x2 = 9; the
solution is x1 = 3.3 and x2 = 1.9. However, x1 + x2 = 5.2 > 4, which can’t be the
case.
1
```
