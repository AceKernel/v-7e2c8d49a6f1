# Tutorial 11, Problem 3: Quadratic concavity and KKT sufficiency

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-11-solutions.md) | [Original PDF](tutorial-11-solutions.pdf)

Topics: lagrange; kkt; convexity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 3

[Original page](tutorial-11-solutions.pdf#page=3)

```text
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

## PDF page 4

[Original page](tutorial-11-solutions.pdf#page=4)

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
