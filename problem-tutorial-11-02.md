# Tutorial 11, Problem 2: Cobb-Douglas choice and an increasing transformation

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-11-solutions.md) | [Original PDF](tutorial-11-solutions.pdf)

Topics: kkt; unconstrained.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 2

[Original page](tutorial-11-solutions.pdf#page=2)

```text
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

[Original page](tutorial-11-solutions.pdf#page=3)

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
```
