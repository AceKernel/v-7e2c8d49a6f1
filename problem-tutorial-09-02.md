# Tutorial 9, Problem 2: Juice-factory linear program, dual and resource values

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-09-solutions.md) | [Original PDF](tutorial-09-solutions.pdf)

Topics: linear-programming; duality; graphs.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 2

[Original page](tutorial-09-solutions.pdf#page=2)

```text
Problem 2
A factory makes two kinds of juices: orange juice and apple juice. Each liter of orange
juice can be sold for $1, while each liter of apple juice can be sold for $2. The production
capacity of the factory limits them to producing a total of 2,000 liters of juice. Each liter of
orange juice requires 1 hour of labor to process and package. Each liter of apple juice requires
8/3 hours of labor to process and package. The company has a total of 4,000 hours of labor
available. Government regulation rations the production of orange juice. The factory has a
license that permits it to produce up to 1,500 gallons of orange juice. What mix of orange
and apple juice should be produced to maximize the revenue of the factory?
The problem of the factory can be formulated as a linear program. Let 𝑥1 denote the
number of liter of orange juice (measured in units of a thousand) to be produced and 𝑥2
be the number of liters of apple juice produced (measured in units of a thousand). Since
a non-negative amount must be produced, 𝑥1, 𝑥2 ≥0. Revenue will be 𝑥1 + 2𝑥2. The total
amount produced 𝑥1 + 𝑥2 must be at most 2, i.e., 𝑥1 + 𝑥2 ≤2. Similarly, the limit on labor
time means that 𝑥1 + (8/3)𝑥2 ≤4. Finally, the government constraint requires that 𝑥1 ≤1.5.
Summarizing, the problem of the factory is
max
𝑥1 + 2𝑥2
s.t.
𝑥1 + 8
3𝑥2 ≤4,
𝑥1 + 𝑥2 ≤2,
𝑥1 ≤3
2,
𝑥1, 𝑥2 ≥0.
2
```

## PDF page 3

[Original page](tutorial-09-solutions.pdf#page=3)

```text
ECON 2050
S2 2026
(a) Use the extreme value theorem to determine whether the problem has a solution.
(b) Use the fundamental theorem of linear programming to find a solution to the linear
program.
(c) Write down the dual of this linear program.
(d) Interpret the dual variables.
(e) Determine whether the optimal value of the dual is the same as the primal above.
Solution:
(a) Because the objective function is linear, it is continuous. The constraint set 𝐷, shaded in
orange in the picture below, is a compact set. Then by the extreme value theorem, the
linear programming problem has a solution.
𝑥1
𝑥2
𝑥1 + 8
3𝑥2 = 4
𝑥1 + 𝑥2 = 2
𝑥1 = 3
2
(0, 0)
(3
2, 0)
( 3
2, 1
2)
( 4
5, 6
5)
(0, 3
2)
𝐷
(b) By the fundamental theorem of linear programming, since a solution exists by part (a),
an extreme point (or vertex or corner) of the constraint set must be a solution. Therefore,
it suffices to compare the value of the objective function 𝑓(𝑥1, 𝑥2) ≡𝑥1 + 2𝑥2 at the five
extreme points: (0, 0), (0, 3/2), (4/5, 6/5), (3/2, 1/2), (3/2, 0). Now
𝑓(0, 0) = 0, 𝑓(0, 3/2) = 3, 𝑓(4/5, 6/5) = 16/5, 𝑓(3/2, 1/2) = 5/2, 𝑓(3/2, 0) = 3/2.
Since 16/5 is the largest, a solution of this linear programming problem is (𝑥∗
1, 𝑥∗
2) =
(4/5, 6/5).
(c) The dual is
min 4𝑦1 + 2𝑦2 + 3
2𝑦3
s.t. 𝑦1 + 𝑦2 + 𝑦3 ≥1,
8
3𝑦1 + 𝑦2 ≥2,
𝑦1 ≥0, 𝑦2 ≥0, 𝑦3 ≥0.
3
```

## PDF page 4

[Original page](tutorial-09-solutions.pdf#page=4)

```text
ECON 2050
S2 2026
(d) The dual variable 𝑦1 can be interpreted as the marginal value of labor, or more specifi-
cally, the relative contribution that one unit of labor makes to the total revenue. Simi-
larly, 𝑦2 and 𝑦3 are the marginal values of total production capacity and production limit
of orange juice, respectively.
Alternatively, one can also interpret each dual variables as the imputed cost of using an
extra unit of each of the resources.
(e) By the duality theorem, since the primal has a solution by part (a), the optimal value of
the primal and the dual must coincide.
```
