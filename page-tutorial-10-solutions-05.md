# Tutorial 10 solutions: P3: Log utility with a quadratic equality and multiplier interpretation

PDF page 5 of 7.

[Page map](map-tutorial-10-solutions.md) | [Original PDF page](tutorial-10-solutions.pdf#page=5) | [Previous](page-tutorial-10-solutions-04.md) | [Next](page-tutorial-10-solutions-06.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
x
y
O
x = 2
y = 2
(2, 5)
(5, 2)
(2, 2)
−5
−4
−3
−2
−1
1
2
3
4
5
6
−5
−4
−3
−2
−1
1
2
3
4
5
6
x2 + y2 = 29
Constraint
Set
The Lagrangian conditions are (for a reference, see the last slide in lecture 10)
−2
x −2λ1x + λ2 = 0
−5
y −2λ1y + λ3 = 0
x2 + y2 −29 = 0
λ2(2 −x) = 0
λ3(2 −y) = 0
Again, we tackle the problem by starting from the two complementary slackness condi-
tions, namely the last two equations above.
If λ2 > 0 and λ3 > 0, the complementary slackness conditions imply x = y = 2, which
violates the equality constraint x2 + y2 = 29, a contradiction.
If λ2 = λ3 = 0, the first two equations above imply that x2 = −1
λ1 and y2 = −5
2λ1. Then
the equality constraint implies that 1 + 5
2 = −29λ1, yielding λ1 = −7
58, which in turn
yields x =
q
58
7 and y =
q
145
7 . Thus, (x∗, y∗, λ∗
1, λ∗
2, λ∗
3) =
q
58
7 ,
q
145
7 , −7
58, 0, 0

satisfies the Lagrange conditions.
Now suppose λ2 = 0 and λ3 > 0. The last equality then implies y = 2; from the equality
constraint x = 5. Plugging these into the first two equalities, we get λ1 = −1
25 and λ3 =
117
50 . Thus, (x∗, y∗, λ∗
1, λ∗
2, λ∗
3) =
5, 2, −1
25, 0, 117
50

satisfies the Lagrange conditions.
Finally, suppose λ3 = 0 and λ2 > 0. The penultimate equality implies that x = 2 and
hence from the equality constraint y = 5. Plugging these into the first two equalities,
5
```
