# Tutorial 11 solutions: P3: Quadratic concavity and KKT sufficiency

PDF page 4 of 4.

[Page map](map-tutorial-11-solutions.md) | [Original PDF page](tutorial-11-solutions.pdf#page=4) | [Previous](page-tutorial-11-solutions-03.md)

Topics: convexity, kkt, lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
2x2 ≤−1. The Lagrange conditions are
−2x1 −x2 −λ1 −2λ2 = 0
−x1 −2x2 + 2λ1 −λ2 = 0
λ1 ≥0,
x1 −2x2 + 1 ≤0,
λ1 (x1 −2x2 + 1) = 0
λ2 ≥0,
2x1 + x2 −2 ≤0,
λ2 (2x1 + x2 −2) = 0.
As usual, we start by discussing the signs of λ1 and λ2.
• λ1 = 0, λ2 = 0.
The first two equalities then reduce to
−2x1 −x2 = 0,
−x1 −2x2 = 0.
But this means that x1 = x2 = 0, which violates the first constraint. A contradiction.
• λ1 > 0, λ2 = 0.
Since λ1 > 0, by complementary slackness, x1 −2x2 = −1. Thus, x1 = 2x2 −1;
plugging this and λ2 = 0 into the first two equalities, we get
−4x2 + 2 −x2 −λ1 = 0
−2x2 + 1 −2x2 + 2λ1 = 0
which can be simplified to
5x2 + λ1 = 2;
4x2 −2λ1 = 1.
Solving this system of equations, we get x2 = 5/14 and λ1 = 3/14; then x1 =
2x2 −1 = −2/7. Thus, (x∗
1, x∗
2, λ∗
1, λ∗
2) = (−2/7, 5/14, 3/14, 0) satisfies the Lagrange
conditions.
• λ1 = 0, λ2 > 0.
Similar to the previous case, since λ2 > 0, by complementary slackness, 2x1 + x2 = 2,
and hence x2 = 2 −2x1. Plugging this and λ1 = 0 into the first two equalities, we get
−2x1 −2 + 2x1 −2λ2 = 0,
−x1 −4 + 4x1 −λ2 = 0.
But solving this system yields λ2 = −1 < 0, a contradiction.
• λ1 > 0, λ2 > 0. Complementary slackness implies that
x1 −2x2 = −1,
2x1 + x2 = 2.
Solving this system, we get x1 = 3/5 and x2 = 4/5. However, since λ1, λ2 > 0, the
condition −2x1 −x2 −λ1 −2λ2 = 0 must be violated.
Thus, (x∗
1, x∗
2, λ∗
1, λ∗
2) = (−2/7, 5/14, 3/14, 0) is the unique point satisfying the Lagrange
conditions. Then since the Lagrange conditions are necessary and sufficient, (x∗
1, x∗
2) =
(−2/7, 5/14) is the unique solution of the maximization problem.
4
```
