# Tutorial 11 solutions: P2: Cobb-Douglas choice and an increasing transformation; P3: Quadratic concavity and KKT sufficiency

PDF page 3 of 4.

[Page map](map-tutorial-11-solutions.md) | [Original PDF page](tutorial-11-solutions.pdf#page=3) | [Previous](page-tutorial-11-solutions-02.md) | [Next](page-tutorial-11-solutions-04.md)

Topics: convexity, kkt, lagrange, unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
If λ > 0, by complementary slackness, 5x + 10y = 500. Consequently, either x > 0
or y > 0, as otherwise 5x + 10y = 0, a contradiction. If x > 0, complementary slackness
implies y = 5λ > 0; similarly, if y > 0, complementary slackness implies x = 10λ > 0.
Thus, it must be that x > 0 and y > 0. Again by complementary slackness, y = 5λ and
x = 10λ. Thus, (x∗, y∗, λ∗) = (50, 25, 5) also satisfies the KKT conditions.
Since the constraint set (i.e., the budget set) is compact and the objective function is
continuous, the extreme value theorem applies, and therefore a solution exists. Then since
the KKT conditions are necessary; that is, every solution must (together with some λ∗≥0)
satisfy the KKT conditions, it suffices to compare the values of the objective function at
(50, 25) and (0, 0). Since u(50, 25) = 1250 > 0 = u(0, 0), we can conclude that (x∗, y∗) =
(50, 25) is the unique solution to the consumer’s problem.
Remark. For KKT conditions, even if there are only two variables and one constraint (ex-
cluding nonnegativity constraints), discussing the signs of x, y, and λ can be daunting. It is
usually helpful to start with a subset of them. In this question, we start from discussing the
sign of λ; in some other questions, discussing the signs of x and y first can also be helpful.
Problem 3
Find a solution to the maximization problem
max
(x1,x2)∈R2 −x2
1 −x1x2 −x2
2
s.t.
−x1 + 2x2 ≥1
2x1 + x2 ≤2.
(Hint. Use the trick used in Tutorial 8 Problem 1 to prove that the objective function is con-
cave. If you have difficulties proving this fact, assume that it is concave and move on.)
Solution: Denoting the objective function by f(x1, x2), note that it can be written as
f (x1, x2) = −

x1 + 1
2x2
2
−3
4x2
2.
Denote f1(x1, x2) = −
x1 + 1
2x2
2, and f2(x1, x2) = −3
4x2
2. Letting g(x1, x2) = x1 + 1
2x2
and h(z) = −z2, we know that g is affine and h is concave. By tutorial 8 problem 1 part
(a), since f1 = h ◦g, f1 is concave. Since f2 is also concave, and the sum of two concave
functions is concave, the objective function must be concave.
Because the objective function is concave and the constraints are linear, we know that
the Lagrange conditions are necessary and sufficient; that is, a point (x∗
1, x∗
2) is a solution
to the maximization problem if and only if there exist Lagrange multipliers λ∗
1, λ∗
2 ≥0 such
that (x∗
1, x∗
2, λ∗
1, λ∗
2) satisfies the Lagrange conditions.
To write down the Lagrange conditions, it is useful to write the first constraint as x1 −
3
```
