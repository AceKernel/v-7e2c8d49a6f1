# Tutorial 9 solutions: P1: Graphical optimisation on different feasible sets; P2: Juice-factory linear program, dual and resource values

PDF page 2 of 6.

[Page map](map-tutorial-09-solutions.md) | [Original PDF page](tutorial-09-solutions.pdf#page=2) | [Previous](page-tutorial-09-solutions-01.md) | [Next](page-tutorial-09-solutions-03.md)

Topics: duality, graphs, linear-programming, unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
By the implicit function theorem, the slope of the line tangent to the constraint set
{(𝑥, 𝑦) ∈ℝ2 ∶𝑥2 + 𝑦2 = 8} at (𝑥, 𝑦) is −2𝑥
2𝑦(as long as 𝑦≠0). Since the slope of
the level curves is 1, we must have −2𝑥
2𝑦= 1 at every point (𝑥, 𝑦) at which a level curve
is tangent to the constraint set. Hence 𝑥= −𝑦and 𝑥2 + 𝑦2 = 8 implies 2𝑥2 = 8 and
𝑥= ±2. The maximum is (2, −2) (at this point, the level curve of level 𝑐= 4 is tangent
to the constraint set.) At (−2, 2), 𝑓has a minimum in the constraint set.
(c) We see that the maximum is (√8, 0), a point on the level curve of level 𝑐= √8
2
-2
c=0
c=1
c=2
c=8
1/2
y
x
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
