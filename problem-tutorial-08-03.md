# Tutorial 8, Problem 3: Existence on a disk and a triangle

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-08-solutions.md) | [Original PDF](tutorial-08-solutions.pdf)

Topics: existence; graphs.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 3

[Original page](tutorial-08-solutions.pdf#page=3)

```text
Problem 3
Use extreme value theorem to show that the following maximization problems have a
solution.
(a) max(x,y)∈C f(x, y), where f(x, y) = 2xy2, and
C = {(x, y) ∈R2 : x2 + y2 ≤1}.
(b) max(x,y)∈D g(x, y), where g(x, y) = 4x + 7y, and
D = {(x, y) ∈R2 : x + 2y ≤3, x ≥0, y ≥0}.
Solution:
(a) Observe that f = 2(pr1)(pr2)(pr2). Since the projections pr1 and pr2 are continuous,
so is their product; moreover, multiplying a function by 2 doesn’t change it continuity.
Thus, the objective function f is continuous.
The set C is closed because it contains all its boundary points (every point in the set
{(x, y) ∈R2 : x2 + y2 = 1} is a boundary point, which is contained in C), and it is also
bounded because for all (x, y) ∈C, ∥(x, y)∥≤1. Therefore, C is compact.
Then by the extreme value theorem, the maximization problem max(x,y)∈C f(x, y) has a
solution.
Graphically, C is the closed ball centered at (0, 0) with radius 1; its boundary is the circle
in black.
x
y
O
(1, 0)
(−1, 0)
(0, 1)
(0, −1)
r = 1
3
```

## PDF page 4

[Original page](tutorial-08-solutions.pdf#page=4)

```text
ECON 2050
S2 2026
(b) Observe that g = 4pr1 + 7pr2. Since the projections pr1 and pr2 are continuous, so
are 4pr1 and 7pr2 (in the future, you can just say that any affine, and therefore linear,
function is continuous). Then because the sum of continuous functions is continuous,
the objective function g is continuous.
The set D is closed because it contains all its boundary points (every point in the set
{(x, y) ∈R2 : x + 2y = 3, x = 0, y = 0} is a boundary point, which is contained in
D), and it is also bounded because for all (x, y) ∈D, ∥(x, y)∥≤3. Thus, D is compact.
Graphically, D is the triangle area in the picture below. The set of boundary points is
the lines in blue and red.
x
y
y = 0
x = 0
x + 2y = 3
O
1
2
3
0.5
1
1.5
```
