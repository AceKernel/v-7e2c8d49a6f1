# Tutorial 9 solutions: automatic text transcript

Original: [Tutorial 9 solutions PDF](tutorial-09-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050
S2 2026
Tutorial 9 Solution
Problem 1
Let 𝑓∶ℝ2 →ℝbe given by 𝑓(𝑥, 𝑦) = 𝑥−𝑦. Solve the following problems graphically:
(a) max𝑥,𝑦∈ℝ𝑓(𝑥, 𝑦)
(b) max𝑥,𝑦∈ℝ𝑓(𝑥, 𝑦)
subject to 𝑥2 + 𝑦2 = 8
(c) max𝑥≥0, 𝑦≥0 𝑓(𝑥, 𝑦)
subject to 𝑥2 + 𝑦2 ≤8
Solution: In all three cases, the level curve of level 𝑐comprises all (𝑥, 𝑦) ∈ℝ2 that satisfy
𝑥−𝑦= 𝑐, or, equivalently, 𝑦= 𝑥−𝑐.
(a) We see that there is no maximum — “we can always increase 𝑐.” That is, the problem has
no solution.
2
-2
c=0
c=1
c=2
y
x
(b) We see that the solution is the tangency point depicted below.
2
-2
c=0
c=1
c=2
-4
4
c=4
(2,-2)
y
x
1
```

## PDF page 2

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

## PDF page 3

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
Problem 3
Consider the linear programming problem
max 2𝑥+ 7𝑦
s.t. 4𝑥+ 5𝑦≤20,
3𝑥+ 7𝑦≤21,
𝑥≥0, 𝑦≥0.
(a) Use the fundamental theorem of linear programming to find a solution to the linear
program; you can assume that a solution exists.
(b) Write down the dual of the linear program.
(c) Suppose the solution to the dual is (𝜆1, 𝜆2) = (0, 1). Then if we change 20 to 20.1 and 21 to
20.8. What is the corresponding change in the optimal value of the objective function?
Solution:
(a) The extreme points (or vertices or corners) of the constraint set are (0, 0), (0, 3), (5, 0),
and (
35
13, 24
13) . To find the solution, we evaluate the value of 𝑓(𝑥, 𝑦) ≡2𝑥+ 7𝑦at each of
the extreme points:
𝑓(0, 0) = 0,
𝑓(0, 3) = 21,
𝑓(5, 0) = 10,
𝑓(
35
13, 24
13) = 238
13 .
Since 21 is the largest, a solution is (𝑥∗, 𝑦∗) = (0, 3).
(b) The dual is
min 20𝜇1 + 21𝜇2
s.t. 4𝜇1 + 3𝜇2 ≥2,
5𝜇1 + 7𝜇2 ≥7,
𝜇1 ≥0, 𝜇2 ≥0.
(c) Recall that the dual variable can be interpreted as the per unit increase in objective func-
tion value from relaxing one of the primal constraints for a sufficiently small amount.
Then by changing 20 to 20.1 and 21 to 20.8, the change in the optimal value of the objec-
tive function is
𝜆1(20.1 −20) + 𝜆2(20.8 −21) = 0(0.1) + 1(−0.2) = −0.2.
4
```

## PDF page 5

```text
ECON 2050
S2 2026
Problem 4
Write down the dual of the following linear programming problems.
(a)
max
𝑥1 + 𝑥2 −3𝑥3
s.t.
𝑥1 + 2𝑥2 −3𝑥3
≤4
4𝑥1 + 5𝑥2 −9𝑥3
≤13
(b)
max
𝑥1 + 𝑥2 −3𝑥3
s.t.
𝑥1 + 2𝑥2 −3𝑥3
= 4
4𝑥1 + 5𝑥2 −9𝑥3
= 13
Solution: Letting
c = (1
1
−3) ,
A = (
1
2
−3
4
5
−9) ,
and
b = (
4
13) ,
the linear programs in parts (a) and (b) can be written as
max c ⋅x
s.t. Ax ≤b
and
max c ⋅x
s.t. Ax = b,
respectively. Now using the observations in lecture 9 slides under the “writing down the
dual” section, their duals are
min y ⋅b
s.t. yA = c, y ≥0,
and
min y ⋅b
s.t. yA = c,
respectively. Therefore, the dual of the problem in part (a) is
min
4𝑦1 + 13𝑦2
s.t.
𝑦1 + 4𝑦2 = 1
2𝑦1 + 5𝑦2 = 1
−3𝑦1 −9𝑦2 = −3
𝑦1 ≥0, 𝑦2 ≥0
and the dual of the problem in part (b) is
min
4𝑦1 + 13𝑦2
s.t.
𝑦1 + 4𝑦2 = 1
2𝑦1 + 5𝑦2 = 1
−3𝑦1 −9𝑦2 = −3
Problem 5 (Extra Practice Problem)
5
```

## PDF page 6

```text
ECON 2050
S2 2026
An electronics firm that produces phones and tablets has two factories that jointly pro-
duce the two goods in the following quantities per hour:
Factory 1
Factory 2
Phones
10
20
Tablets
25
25
The firm receives an order for 300 phones and 500 tablets. The costs of operating the two
factories are $10000 and $8000 per hour, respectively.
(a) Formulate the linear programming problem of minimizing the total cost of meeting this
order.
(b) Write down the equivalent maximization problem, and then find its dual.
Solution:
(a) Let 𝑥1 and 𝑥2 denote the number of hours for which the two factories operate to produce
the order. Then the above table tells us that a total of 10𝑥1 + 20𝑥2 phones is produced,
as well as 25𝑥1 + 25𝑥2 tablets. Because 300 phones and 500 tablets are required, the pair
(𝑥1, 𝑥2) must satisfy
10𝑥1 + 20𝑥2 ≥300
25𝑥1 + 25𝑥2 ≥500
In addition, of course, 𝑥1 ≥0 and 𝑥2 ≥0. The total cost of operating the two factories for
𝑥1 and 𝑥2 hours, respectively, is 10000𝑥1 + 8000𝑥2. The problem is, therefore,
min 10000𝑥1 + 8000𝑥2
s.t.
{
10𝑥1 + 20𝑥2 ≥300
25𝑥1 + 25𝑥2 ≥500 and 𝑥1 ≥0, 𝑥2 ≥0
(b) The linear programming problem above is equivalent to (also changed ≥to ≤in the
constraints)
max −10000𝑥1 −8000𝑥2
s.t.
{
−10𝑥1 −20𝑥2 ≤−300
−25𝑥1 −25𝑥2 ≤−500 and 𝑥1 ≥0, 𝑥2 ≥0
Its dual is
min −300𝑦1 + −500𝑦2
s.t.
{
−10𝑦1 −25𝑦2 ≥−10000
−20𝑦1 −25𝑦2 ≥−8000
and 𝑦1 ≥0, 𝑦2 ≥0
6
```
