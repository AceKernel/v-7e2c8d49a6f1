# Tutorial 10, Problem 2: Equality-circle constraint and existence

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-10-solutions.md) | [Original PDF](tutorial-10-solutions.pdf)

Topics: lagrange; existence.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 2

[Original page](tutorial-10-solutions.pdf#page=2)

```text
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

[Original page](tutorial-10-solutions.pdf#page=3)

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
```
