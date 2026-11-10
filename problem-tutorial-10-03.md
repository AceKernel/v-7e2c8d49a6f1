# Tutorial 10, Problem 3: Log utility with a quadratic equality and multiplier interpretation

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-10-solutions.md) | [Original PDF](tutorial-10-solutions.pdf)

Topics: lagrange.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 3

[Original page](tutorial-10-solutions.pdf#page=3)

```text
Problem 3
(a) For x > 0, y > 0, z > 0, write down the Lagrange conditions the constrained maximiza-
tion problem
max
(x,y,z)∈R3
+
2 ln x + 5 ln y + ln z
s.t.
x2 + y2 + z = 32,
and find the unique point satisfying the Lagrange conditions.
(b) Assuming that the point you found is indeed the unique solution to the maximization prob-
lem above, use your answer to part (a) to provide an approximation of the optimal value
of the maximization problem
max
(x,y,z)∈R3 2 ln x + 5 ln y + ln z
s.t.
x2 + y2 + z = 32.1
Do not solve this maximization problem. Briefly explain your reasoning.
(c) (Extra Practice Problem) For x ≥2, y ≥2, z = 3, solve (if there is a solution) the
constrained minimization problem
min
x≥2,y≥2,z>0 2 ln x + 5 ln y + ln z
s.t.
x2 + y2 + z = 32;
z = 3
If there is no solution, explain why (you can assume that every solution of the problem
must satisfy the Lagrange conditions).
3
```

## PDF page 4

[Original page](tutorial-10-solutions.pdf#page=4)

```text
ECON 2050
S2 2026
Solution:
(a) Letting g(x, y, z) = x2 + y2 + z then ∇g(x, y, z) = (2x, 2y, 1) ̸= (0, 0, 0). Therefore,
{∇g(x, y, z)} is linearly independent for every (x, y, z) in the constraint set. Thus, the
Lagrange conditions are necessary. The Lagrange conditions are
2
x −2λx = 0
⇔
x2 = 1
λ
5
y −2λy = 0
⇔
y2 = 5
2λ
1
z −λ = 0
⇔
z = 1
λ
x2 + y2 + z −32 = 0
Plugging the first three equations into the last gives
1 + 5
2 + 1 −32λ = 0
⇔
λ = 9
64;
plugging this back to the first three equations, we get that the unique point satisfying
the Lagrange condition is
(x∗, y∗, z∗, λ∗) =
 
8
3, 8
√
5
3
√
2, 64
9 , 9
64
!
.
(b) Let V (32) be the optimal value of the problem in part (a), and let V (32.1) be the optimal
value of the problem in this part. Using the multiplier λ∗corresponding to the solution
from part (a), and recall that λ∗can be interpreted as the per unit increase in objective
function value from the constraint for a sufficiently small amount:
V (32.1) ≈V (32)+0.1λ∗= 2(ln 8−ln 3)+5(ln 8+ln
√
5−ln 3−ln
√
2)+ln 64−ln 9+ 9
640
(The exact calculation doesn’t really matter; what matters is the first part.)
(c) The problem is equivalent to
max
(x,y)∈R2 −2 ln x −5 ln y −ln 3
s.t.
x2 + y2 = 29;
2 −x ≤0;
2 −y ≤0
The constraint set is visualized below; we see that it is compact. Because the objective
function is continuous, a solution exists.
4
```

## PDF page 5

[Original page](tutorial-10-solutions.pdf#page=5)

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

## PDF page 6

[Original page](tutorial-10-solutions.pdf#page=6)

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
```
