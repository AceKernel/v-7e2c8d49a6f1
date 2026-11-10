# Tutorial 10 solutions: P3: Log utility with a quadratic equality and multiplier interpretation; P4: Parameter-dependent disk constraint: extra practice

PDF page 6 of 7.

[Page map](map-tutorial-10-solutions.md) | [Original PDF page](tutorial-10-solutions.pdf#page=6) | [Previous](page-tutorial-10-solutions-05.md) | [Next](page-tutorial-10-solutions-07.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
we get Also λ1 = −1
10 and λ2 = 3
5. Thus, (x∗, y∗, λ∗
1, λ∗
2, λ∗
3) =
2, 5, −1
10, 3
5, 0

satisfies
the Lagrange conditions.
The value of the objective function at the three candidate solutions are
f
 r
58
7 ,
r
145
7
!
= −2 ln
r
58
7 −5 ln
r
145
7
−ln 3
f(5, 2) = −2 ln 5 −5 ln 2 −ln 3
f(2, 5) = −2 ln 2 −5 ln 5 −ln 3
Since a solution exists, and every solution must satisfy the Lagrange conditions, the
points which the objective function obtains the highest value are solutions. Comparing
the values, we reach the conclusion that the unique solution is (x∗, y∗) = (5, 2).
Problem 4 (Extra Practice Problem)
Consider the maximization problem
max
(x,y)∈R2 2 −(x −1)2 −ey2
subject to
x2 + y2 ≤a.
Write down the Lagrange conditions, then find the only point that satisfies the Lagrange
conditions.
(Hint. Distinguishing between the cases a ∈(0, 1) and a ≥1.)
Solution: The Lagrange conditions are
−2(x −1) −2λx = 0
−2yey2 −2λy = 0
x2 + y2 ≤a
λ ≥0
λ(x2 + y2 −a) = 0
The first two equations can be simplified to
(x −1) + λx = 0,
(1)
2y(ey2 + λ) = 0.
(2)
We analyze the solution by considering two cases based on the complementary slackness
condition, namely the last equation in the Lagrange conditions.
Case 1: The constraint is not binding (λ = 0).
If λ = 0, the complementary slackness
condition is satisfied.
• From equation (2): 2y(ey2 + 0) = 0 =⇒2yey2 = 0. Since ey2 > 0, we must have
y = 0.
• From equation (1): (x −1) + 0 · x = 0 =⇒x −1 = 0 =⇒x = 1.
6
```
