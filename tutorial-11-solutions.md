# Tutorial 11 solutions: automatic text transcript

Original: [Tutorial 11 solutions PDF](tutorial-11-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050
S2 2026
Tutorial 11 Solution
Problem 1
Consider the following nonlinear programming problem
max 2x −2y2
s.t.
2x −y ≤5, y ≤4, x ≥0, y ≥0.
(a) Try to solve (at least roughly) the problem graphically.
(b) Solve the problem using the KKT approach.
Solution:
(a) The level curve of the objective function of level C is defined by the equation x = y2+ 1
2C.
You have to draw quite precisely to see the exact solution: it is (x∗, y∗) = (21/8, 1/4).
C
y = −5 + 2x
y = 4
2x −2y2 = 5.125
x
y
−1
0
1
2
3
4
5
−1
0
1
2
3
4
5
(b) Because the constraint functions are all affine, the KKT conditions are necessary.
The KKT conditions are
2 −2λ1 ≤0,
x ≥0,
x(2 −2λ1) = 0
−4y + λ1 −λ2 ≤0,
y ≥0,
y(−4y + λ1 −λ2) = 0
2x −y −5 ≤0,
λ1 ≥0,
λ1(2x −y −5) = 0
y −4 ≤0,
λ2 ≥0,
λ2(y −4) = 0
We see that
• x > 0 and λ1 = 1: Because 2 −2λ1 ≤0, we must have λ1 > 0. Hence by
complementary slackness [λ1(2x −y −5) = 0], 2x −y = 5. But this implies that
x = 0: if x = 0, 2(0) −y = 5 and thus y = −5 < 0, a contradiction. Hence x > 0;
by complementary slackness [x(2 −2λ1) = 0], we have λ1 = 1.
1
```

## PDF page 2

```text
ECON 2050
S2 2026
• Now it remains to discuss the signs of y and λ2. Suppose y = 0, then Thus y > 0:
Suppose that y = 0. Then −4y + λ1 −λ2 ≤0 becomes 1 = λ1 ≤λ2, so λ2 > 0.
Again by complementary slackness [λ2(y−4) = 0], we have y = 4, a contradiction.
• Thus, we must have y > 0. By complementary slackness, −4y + λ1 −λ2 = 0. Now
suppose λ2 = 0. Then y = 1/4; since 2x−y = 5, x = 21/8. Thus, (x∗, y∗, λ∗
1, λ∗
2) =
(21/8, 1/4, 1, 0) satisfies the KKT conditions.
• Now suppose λ2 > 0. By complementary slackness, y = 4. Then −4y+λ1−λ2 = 0
yields (since y = 4 and λ1 = 1) λ2 = −15 < 0, a contradiction.
Therefore, the only point satisfying the KKT conditions is (x∗, y∗, λ∗
1, λ∗
2) = (21/8, 1/4, 1, 0).
Since the objective function is continuous and the constraint set is compact, the extreme
value theorem applies, and therefore a solution exists. Then since the KKT conditions
are necessary; that is, every solution must (together with some λ∗
1 ≥0 and λ∗
2 ≥0)
satisfy the KKT conditions, we can conclude that (x∗, y∗) = (21/8, 1/4) is the unique
solution.
Remark. As illustrated by this question, after you wrote down the KKT conditions, it is usu-
ally useful to stare at the conditions and think about whether there are conditions that offer
clear guidance of the signs of the variables. Here, the condition 2 −2λ1 ≤0 indicates that
λ1 > 0.
Problem 2
Let u : R2
+ →R given by u(x, y) = √xy be a consumer’s utility function, where x and y
are the quantities of the two goods available to the consumer. The per unit price of the goods
are $5 (for X) and $10 (for Y ), respectively, and the consumer has $500 available. Formulate
and solve the optimization problem of the consumer.
Solution: The consumer’s problem is
max
(x,y)∈R2
+
u(x, y) = √xy
s.t.
5x + 10y ≤500, x ≥0, y ≥0.
Since √· : R →R is a strictly increasing function, the solutions to the consumer’s problem
coincide with those of
max
(x,y)∈R2
+
xy
s.t.
5x + 10y ≤500, x ≥0, y ≥0,
and we can solve the latter problem instead. Since the constraint functions are all affine, the
KKT conditions are necessary.
We write down the KKT conditions
y −5λ ≤0,
x (y −5λ) = 0,
x ≥0
x −10λ ≤0,
y(x −10λ) = 0,
y ≥0
5x + 10y −500 ≤0,
λ(5x + 10y −500) = 0,
λ ≥0
If λ = 0 then by y ≤5λ and x ≤10λ, (x, y) = (0, 0). The point (x∗, y∗, λ∗) = (0, 0, 0)
satisfies the KKT conditions.
2
```

## PDF page 3

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

## PDF page 4

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
