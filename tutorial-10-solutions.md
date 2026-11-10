# Tutorial 10 solutions: automatic text transcript

Original: [Tutorial 10 solutions PDF](tutorial-10-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050
S2 2026
Tutorial 10 Solution
Problem 1
Consider the maximization problem
max
(x,y)∈R2 −(x1 −4)2 −(x2 −4)2
subject to
x1 + x2 ≤4
and
x1 + 3x2 ≤9.
(a) Are the Lagrange conditions necessary? That is, is it true that every solution of the
maximization problem, if exists, must satisfy the Lagrange conditions?
(b) Write down the Lagrange conditions for this problem.
(c) Find all points that satisfy the Lagrange conditions.
Solution:
(a) The Lagrange conditions are necessary because all constraint functions are affine.
(b) The Lagrange conditions are
−2 (x1 −4) −λ1 −λ2 = 0
−2 (x2 −4) −λ1 −3λ2 = 0
x1 + x2 ≤4, λ1 ≥0, and λ1 (x1 + x2 −4) = 0
x1 + 3x2 ≤9, λ2 ≥0, and λ2 (x1 + 3x2 −9) = 0
(c) We start from the two complementary slackness conditions, λ1 (x1 + x2 −4) = 0 and
λ2 (x1 + 3x2 −9) = 0, by discussing the signs of λ1 and λ2. There are four cases:
• λ1 = λ2 = 0. In this case, the first two equations of the Lagrange conditions above
indicate that x1 = x2 = 4, but this violates the constraint x1+x2 ≤4, and therefore
can’t be the case.
• λ1 > 0 and λ2 = 0. In this case, the first two equations of the Lagrange conditions
above indicate that
x1 = x2 = 4 −λ1/2.
Because λ1 > 0, complementary slackness implies that x1 +x2 = 4. Plugging x1 =
x2 in, we get x1 = x2 = 2, which also satisfies x1+3x2 ≤9. Thus, (x∗
1, x∗
2, λ∗
1, λ∗
2) =
(2, 2, 4, 0) satisfies the Lagrange conditions.
• λ1 = 0 and λ2 > 0. In this case, the first line of the Lagrange conditions can be
written as λ2 = −2(x1 −4); plug into the second line, we get
−2(x2 −4) + 6(x1 −4) = 0
⇔
3x1 −x2 = 8.
Now we have two equations and two unknowns: 3x1 −x2 = 8, x1 + 3x2 = 9; the
solution is x1 = 3.3 and x2 = 1.9. However, x1 + x2 = 5.2 > 4, which can’t be the
case.
1
```

## PDF page 2

```text
ECON 2050
S2 2026
• λ1 > 0 and λ2 > 0. Complementary slackness imply that we have two equations
and two unknowns: x1 + x2 = 4, x1 + 3x2 = 9; the solution is x1 = 1.5 and
x2 = 2.5. Then the first two equations of the Lagrange conditions become
5 −λ1 −λ2 = 0
3 −λ1 −3λ2 = 0
implying that λ1 = 6 and λ2 = −1, which violates the condition λ2 ≥0.
Thus, the unique point that satisfies the Lagrange conditions is (x∗
1, x∗
2, λ∗
1, λ∗
2) = (2, 2, 4, 0).
Note. We can solve this problem graphically:
x1
x2
(x∗
1, x∗
2) = (2, 2)
x1 + 3x2 = 9
x1 + x2 = 4
0
4
9
Level curves of −(x1 −4)2 −(x2 −4)2
Indeed, the unique solution is (x∗
1, x∗
2) = (2, 2), confirming that every solution must satisfy
the Lagrange conditions.
Problem 2
Consider the maximization problem
max
(x,y)∈R2 x −y
subject to
x2 + y2 = 8
(a) Does a solution to this maximization problem exist? Explain.
(b) Find all solutions to this maximization problem.
Solution:
(a) Since the objective function is linear, it is continuous. Moreover, the constraint set C is
compact because it is the circle centered at the origin with radius 2
√
2. By the extreme
value theorem, a solution exists.
(b) Define the constraint function g : R2 →R by g(x, y) = x2+y2−8. Note that ∇g(x, y) ̸=
(0, 0) for all (x, y) ∈C = {(x, y) ∈R2 :
x2 + y2 = 8} as ∇g(x, y) = (2x, 2y) =
(0, 0) only if (x, y) = (0, 0) /∈C. Thus, {∇g(x, y)} is linearly independent for all
(x, y) ∈C. Therefore, the Lagrange conditions are necessary; i.e., every solution to the
maximization problem must satisfy the Lagrange conditions.
2
```

## PDF page 3

```text
ECON 2050
S2 2026
The Lagrange conditions are
1 −2λx = 0
−1 −2λy = 0
x2 + y2 −8 = 0
From the first equation, λ ̸= 0. Therefore, the first two equation together imply that
y = −x. The third equation then implies 2x2 = 8 and x = ±2. Consequently, either
x = 2 and y = −2, or x = −2 and y = 2. Plugging x = 2 and x = −2 into the
first equation, we get λ = 1/4 and λ = −1/4, respectively. Thus, there are two points
satisfying the Lagrange conditions:
(x∗
1, y∗
1, λ∗
1) =

2, −2, 1
4

(x∗
2, y∗
2, λ∗
2) =

−2, 2, −1
4

Evaluate the function at (x∗
1, y∗
1) = (2, −2) and (x∗
2, y∗
2) = (−2, 2):
f(x∗
1, y∗
1) = f (2, −2) = 4
f(x∗
2, y∗
2) = f (−2, 2) = −4
Because the Lagrange conditions are necessary and a solution exists by part (a), the
points satisfy the Lagrange conditions and yield the highest value of the objective func-
tion is the solutions. Thus, (x∗
1, y∗
1) = (2, −2) is the unique solution.
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

## PDF page 7

```text
ECON 2050
S2 2026
This gives the candidate point (1, 0). The constraint requires
12 + 02 ≤a =⇒1 ≤a
So, if a ≥1, the point (x∗, y∗, λ∗) = (1, 0, 0) satisfies Lagrange conditions; otherwise it
doesn’t.
Case 2: The constraint is binding (λ > 0).
If λ > 0, the complementary slackness condition
requires x2 + y2 −a = 0.
• From equation (2), 2y(ey2 + λ) = 0. Since λ > 0 and ey2 > 0, their sum is positive.
Therefore, we must have y = 0.
• Substitute y = 0 into the binding constraint: x2 + 02 = a =⇒x = ±√a.
• We use equation (1) to find the valid value for x:
(x −1) + λx = 0 =⇒λ = 1 −x
x
• Since we are in the case where λ > 0, we require 1−x
x
> 0.
– Testing x = √a: We need λ = 1−√a
√a
> 0. Since √a > 0 (for a > 0), this requires
1 −√a > 0 =⇒1 > a.
– Testing x = −√a: We need 1−(−√a)
−√a
> 0, which is 1+√a
−√a > 0. This is never true
as the numerator is positive and the denominator is negative.
The only valid candidate point in this case is (x∗, y∗, λ∗) = (√a, 0, (1/√a −1))), which
satisfies the Lagrange conditions for 0 ≤a < 1.
To summarize,
• If a ≥1, the unique point satisfying the Lagrange conditions is (x∗, y∗, λ∗) = (1, 0, 0)
with a maximum value of 1.
• If 0 ≤a < 1, the unique point satisfying the Lagrange conditions is (x∗, y∗, λ∗) =
(√a, 0, (1/√a −1)).
7
```
