# Tutorial 10 solutions: P2: Equality-circle constraint and existence; P3: Log utility with a quadratic equality and multiplier interpretation

PDF page 3 of 7.

[Page map](map-tutorial-10-solutions.md) | [Original PDF page](tutorial-10-solutions.pdf#page=3) | [Previous](page-tutorial-10-solutions-02.md) | [Next](page-tutorial-10-solutions-04.md)

Topics: existence, lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
