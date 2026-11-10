# Tutorial 11 solutions: P1: Nonnegative KKT with linear constraints; P2: Cobb-Douglas choice and an increasing transformation

PDF page 2 of 4.

[Page map](map-tutorial-11-solutions.md) | [Original PDF page](tutorial-11-solutions.pdf#page=2) | [Previous](page-tutorial-11-solutions-01.md) | [Next](page-tutorial-11-solutions-03.md)

Topics: kkt, unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
