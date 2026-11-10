# Tutorial 11, Problem 1: Nonnegative KKT with linear constraints

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-11-solutions.md) | [Original PDF](tutorial-11-solutions.pdf)

Topics: kkt.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-11-solutions.pdf#page=1)

```text
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

[Original page](tutorial-11-solutions.pdf#page=2)

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
```
