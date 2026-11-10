# Lecture 9: automatic text transcript

Original: [Lecture 9 PDF](lecture-09.pdf). Topic: Linear programming, duality and shadow prices.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050  Mathematical Economics
Optimization II: Linear Programming
ECON 2050  Optimization II
1 / 26
```

## PDF page 2

```text
Linear programming
In this lecture we look at a special class of optimization problems.
The problem of optimizing a linear function subject to linear inequality and equality constraints
is called linear programming (LP).
A (running) example of linear programming problem (linear program for short):
max
x1 + 2x2
s.t.
x1 + 3x2 ≤4,
x1 + x2 ≤2,
x1, x2 ≥0.
In other words, in LP the objective function is linear, and the constraint set is delineated by a
set of linear inequalities and equalities.
ECON 2050  Optimization II
2 / 26
```

## PDF page 3

```text
Example: (For simplicity, the numbers are unrealistic.) A bakery makes both bread and cakes.
From selling a box of bread, the bakery makes prots of $1, and the prots from selling a
box of cakes is $2.
Each box of bread requires 1 unit of labor, and each box of cakes requires 3 units of labor;
there is 4 units of labor available in total.
The production capacity of the bakery limits it to produce no more than 2 boxes of bread
and cakes.
Question: how many boxes of bread and cakes should be produced to maximize the prots of
the bakery?
Denote the numbers of boxes of bread and cakes by x1 ≥0 and x2 ≥0, respectively.
Prots: x1 + 2x2
Labor constraint: x1 + 3x2 ≤4
Production capacity constraint: x1 + x2 ≤2
Therefore, the bakery's prot maximization problem is exactly the linear program on the
previous slide.
ECON 2050  Optimization II
3 / 26
```

## PDF page 4

```text
The linear program can also be written as max(x1,x2)∈D x1 + 2x2, where
D = {(x1, x2) ∈R2 : x1 + 3x2 ≤4, x1 + x2 ≤2, x1 ≥0, x2 ≥0}.
We call a point in the constraint set feasible for the linear program.
x1
x2
1
2
3
4
0.5
1
1.5
2
x1 + 3x2 = 4
x1 + x2 = 2
D
Observe that D is a convex set; more generally, if all constraints are linear inequalities and
equalities, the constraint set is convex.
In other words, the constraint set of any linear program is convex.
ECON 2050  Optimization II
4 / 26
```

## PDF page 5

```text
Extreme points
Denition
Let S ⊆Rn be a convex set. An extreme point of S is a point that cannot be expressed as a
convex combination of any other points in S.
Example: The extreme points of D = {(x1, x2) ∈R2 : x1 +3x2 ≤4, x1 +x2 ≤2, x1 ≥0, x2 ≥0}
are (0, 0), (0, 4
3), (2, 0), and (1, 1).
x1
x2
(0, 0)
(2, 0)
(0, 4
3)
(1, 1)
D
In linear programming, the constraint set is a polyhedron (i.e., a generalized polygon), and its
extreme points are the corners or vertices.
ECON 2050  Optimization II
5 / 26
```

## PDF page 6

```text
Dene f (x1, x2) = x1 + 2x2. Since ∇f (x1, x2) = (1, 2) ̸= (0, 0) for every (x1, x2) ∈R2, there is
no critical points in the interior of D.
This fact is more generally true for any nontrivial linear program.
Therefore, to search for solutions/maxima, it suces to look at boundary points.
Graphical analysis reveals that the unique solution/maximum is extreme point (1, 1).
x1
x2
1
2
3
4
0.5
1
1.5
2
(1, 1)
D
purple lines are level curves of f
In fact, for any linear program that has a solution, an extreme point of the constraint set must
be a solution.
ECON 2050  Optimization II
6 / 26
```

## PDF page 7

```text
General setup and terminology
Every linear programming problem can be written in the following standard form:
max c · x
s.t.
Ax ≤b
x ≥0
Or more compactly, max{c · x : Ax ≤b, x ≥0}.
If xj doesn't have to be non-negative, substitute xj = x+
j −x−
j , where x+
j , x−
j
≥0.
If the objective is min c · x then replace it with max −c · x.
If the i-th constraint is ∑︁n
j=1 aijxj ≥bi, replace it by −∑︁n
j=1 aijxj ≤−bi.
If the i-th constraint is ∑︁n
j=1 aijxj = bi, replace it by two inequality constraints:
∑︁n
j=1 aijxj ≤bi and −∑︁n
j=1 aijxj ≤−bi.
Suppose ˜x is in the constraint set. Then if a constraint holds with equality, say that this
constraint binds at ˜x; if instead the constraint holds with strict inequality, we say it is slack at
˜x.
ECON 2050  Optimization II
7 / 26
```

## PDF page 8

```text
Example: Let us revisit the example at the beginning:
max
x1 + 2x2
s.t.
x1 + 3x2 ≤4,
x1 + x2 ≤2,
x1, x2 ≥0.
In this example, c = (1, 2), A =
(︃1
3
1
1
)︃
, and b = (4, 2).
Recall that a linear function is continuous, and therefore if the constraint set
D = {x ∈Rn : Ax ≤b, x ≥0}
is compact, the linear program has a solution.
ECON 2050  Optimization II
8 / 26
```

## PDF page 9

```text
Fundamental theorem of linear programming
First, we formalize the observation suggested by the example: A maximum is an extreme point.
Theorem (Fundamental Theorem of Linear Programming)
Suppose the linear program max{c · x : Ax ≤b, x ≥0} has a solution. Then an extreme point
of the constraint set is a solution.
Example: Revisiting the example from the beginning:
Observe that the constraint set is compact, and therefore a solution exists.
By the fundamental theorem of linear programming, it suces to search within the set of
extreme points of the constraint set D.
The extreme points are (0, 0), (0, 4
3), (2, 0), and (1, 1), and
f (0, 0) = 0,
f
(︃
0, 4
3
)︃
= 8
3,
f (2, 0) = 2,
and
f (1, 1) = 3.
Thus, (1, 1) is a solution.
ECON 2050  Optimization II
9 / 26
```

## PDF page 10

```text
Going back to our bakery example,
max
x1 + 2x2
s.t.
x1 + 3x2 ≤4,
x1 + x2 ≤2,
x1, x2 ≥0.
In an attempt to solve this problem, we can produce upper bounds on its optimal value V :
Since x1 + 2x2 ≤x1 + 3x2 ≤4, we know V ≤4.
Since x1 + 2x2 ≤(2/3)(x1 + 3x2) + (1/3)(x1 + x2) ≤(2/3)4 + (1/3)2 = 10/3, V ≤10/3.
Since x1 + 2x2 ≤(1/2)(x1 + 3x2) + (1/2)(x1 + x2) ≤(1/2)4 + (1/2)2 = 3, we know
V ≤3.
In each of these cases we take a non-negative linear combination of the constraints, looking for
better and better upper bounds on the maximum possible value of the objective function
x1 + 2x2.
ECON 2050  Optimization II
10 / 26
```

## PDF page 11

```text
We can formalize this process by letting y1 and y2 be the coecients of our linear combination.
We must have
y1 + y2
≥1,
3y1 + y2
≥2,
y1, y2
≥0,
and we seek to minimize 4y1 + 2y2.
We obtained another linear program!
We refer to this new linear program as the dual and the original one as the primal.
Recall that we designed the dual to serve as a method of constructing an upper bound on the
optimal value of the primal.
If (y1, y2) is feasible for the dual, and (x1, x2) is feasible for the primal, then by
construction x1 + 2x2 ≤4y1 + 2y2.
If we can nd feasible (x∗
1, x∗
2) and (y ∗
1 , y∗
2 ) that make these equal, we know we have found
the optimal values of both programs. In fact, (x ∗
1, x∗
2) = (1, 1) and (y ∗
1 , y∗
2 ) = (1/2, 1/2).
ECON 2050  Optimization II
11 / 26
```

## PDF page 12

```text
Duality
More generally, consider the standard form of a linear programming problem
max c · x
s.t. Ax ≤b, x ≥0.
(P)
Taking a linear combination of the constraints with weights y = (y1, . . . , ym) can be written as
yA; since we need to nd an upper bound, it must be that yA ≥c.
Since x ≥0, we have yAx ≥c · x.
Then because Ax ≤b, c · x ≤yAx ≤y · b. Thus, y · b is an upper bound on objective
function value.
Therefore, the problem of nding the smallest such upper bound is
min y · b
s.t. yA ≥c, y ≥0.
(D)
We call problem (D) the dual and problem (P) the primal.
Denote the optimal values of (P) and (D) by V and W , respectively.
Since c · x ≤y · b, we have V ≤W ; this is known as weak duality.
ECON 2050  Optimization II
12 / 26
```

## PDF page 13

```text
Duality theorem
Theorem (Strong duality)
If either the primal or the dual has a solution, then V = W .
Some geometric intuition based on the bakery example:
Recall that the bakery's problem can be written as max c · x s.t. Ax ≤b, x ≥0 by letting
c =
(︁
1
2
)︁
,
A =
(︃1
3
1
1
)︃
,
and
b =
(︃4
2
)︃
.
Denote the rst and the second row of A by a1 and a2, respectively.
At the solution x∗= (x∗
1, x∗
2) = (1, 1), both resource constraints (labor and capacity)
bind.
Also, a1 and a2 are the directions of increase of the two resource constraints,
respectively; and c is the direction of increase of the level curve of the objective function
ECON 2050  Optimization II
13 / 26
```

## PDF page 14

```text
Geometric intuition continued:
x1
x2
(1, 1)
(1, 3)
(1, 2)
O
x1
x2
x1 + 3x2 = 4
x1 + x2 = 2x1 + 2x2 = 3
(1, 1)
(1, 3)
(1, 2)
D
The discussion in the previous slide implies that c is in the cone generated by {a1, a2}.
Therefore, there exists y ∗= (y∗
1 , y∗
2 ) ≥0 such that c = y ∗
1 a1 + y∗
2 a2.
Since the two resource constraints bind at x ∗, which can be written as a1 · x∗= b1 and
a2 · x∗= b2, where b = (b1, b2).
But then c · x∗= (y∗
1 a1 + y∗
2 a2) · x∗= y∗
1 a1x∗+ y∗
2 a2x∗= y∗
1 b1 + y∗
2 b2 = y ∗· b,
implying V = W .
ECON 2050  Optimization II
14 / 26
```

## PDF page 15

```text
A proof of the duality theorem
Suppose that the primal has a solution; the argument starting from the dual having a solution
is analogous. By weak duality, V ≤W ; it suces to show that V ≥W .
If there exists a vector x ≥0 such that Ax ≤b and c · x ≥W , then we have V ≥W .
In other words, it suces to show that the system of inequalities c · x ≥W , Ax ≤b, and
x ≥0 has a solution. Also, c · x ≥W is equivalent to −c · x ≤−W .
Suppose, toward contrary, that the system −c · x ≤−W , Ax ≤b, and x ≥0 has no
solution; equivalently, the system
(︃A
−c
)︃
x ≤
(︃b
−W
)︃
has no non-negative solution.
Then its Farkas alternative
(︁
y
λ
)︁(︃A
−c
)︃
≥0,
(︁
y
λ
)︁(︃b
−W
)︃
< 0,
and
(︁
y
λ
)︁
≥0.
must have a solution.
ECON 2050  Optimization II
15 / 26
```

## PDF page 16

```text
The Farkas alternative can be written as
yA −λc ≥0,
y · b −λW < 0,
y ≥0,
and
λ ≥0;
denote a solution by
(︁
y ∗
λ∗)︁
.
Observe that λ∗> 0: if instead λ∗= 0, the system above reduces to
yA ≥0,
y · b < 0,
and
y ≥0,
which is the Farkas alternative of the system Ax ≥b and x ≥0.
Since it has a solution y ∗, the Farkas lemma implies that the system Ax ≥b and x ≥0
has no solution, violating the assumption that the primal has a solution. Thus, λ∗> 0.
Let ˆy ≡y ∗/λ∗; this is well-dened because λ∗> 0. The system at the top implies
ˆy · A ≥c,
ˆy ≥0,
and
ˆy · b < W ,
showing that ˆy is feasible for the dual and the value of the dual objective function at ˆy is
strictly below W , contradicting the assumption that W is the optimal value of the dual.
ECON 2050  Optimization II
16 / 26
```

## PDF page 17

```text
Interpreting the dual
A benet of studying the dual is that it can help with solving the primal problem.
For example, a problem with many variables and a few constraints can be reduced to
another with a few variables and many constraints, which is usually much simpler.
The Lagrangian approach of constrained optimization you learned in ECON1050 and/or
ECON2010 is a generalization of duality: the Lagrange conditions stem from the dual of
the optimization problem we study.
An arguably more powerful aspect of duality theory is that; however, the dual reveals valuable
insights that are not immediately apparent in the primal.
For studying economics, nance, and business, this aspect is usually more important than
the computational benets mentioned above.
In what follows we illustrate this by going back once again to the bakery example.
ECON 2050  Optimization II
17 / 26
```

## PDF page 18

```text
Consider the example of a bakery on slide 3, with an extra twist that since cakes need to be
refrigerated, there is an extra storage constraint that the at most 6/5 boxes of cakes can be
produced in a day. Thus, the linear program becomes
max
x1 + 2x2
s.t.
x1 + 3x2 ≤4,
x1 + x2 ≤2,
x2 ≤6
5,
x1, x2 ≥0.
It can be veried that the unique optimal solution is still (x ∗
1, x∗
2) = (1, 1).
x1
x2
1
2
3
4
0.5
1
1.5
2
x1 + 3x2 = 4
x1 + x2 = 2
x2 = 6
5
D
(1, 1)
ECON 2050  Optimization II
18 / 26
```

## PDF page 19

```text
Now suppose an entrant wishes to buy the bakery from the current owner. She oers a per unit
price for each resource that the owner possesses.
Suppose the entrant intends to oer prices y1, y2, and y3 for each unit of labor,
production capacity, and storage space.
Because a box of bread requires a unit of labor, a unit of production capacity, and no
(fridge) storage space, the owner will get y1 + y2 for all the resources needed to produce a
box of bread.
There was originally $1 prot for each box of bread, so for this to be a protable
transaction, the owner requires y1 + y2 ≥1.
Similarly, because a box of cakes requires 3 units of labor, a unit of production capacity,
and a unit of (fridge) storage space, the owner will get 3y1 + y2 + y3 for all the resources
needed to produce a box of cakes.
There were originally $2 prots for each box of cakes, so for this to be a protable
transaction, the owner requires 3y1 + y2 + y3 ≥2.
ECON 2050  Optimization II
19 / 26
```

## PDF page 20

```text
Now the entrant wants to buy the owner's resources as inexpensively as possible while having
the owner accept the oer.
The total cost of 4 units of labor, 2 units of production capacity, and 6/5 units of storage
space, is 4y1 + 2y2 + 6
5y3.
Therefore, the entrant's problem is
min
4y1 + 2y2 + 6
5y3
s.t.
y1 + y2 ≥1,
3y1 + y2 + y3 ≥2,
y1, y2, y3 ≥0.
It is not dicult to verify that the entrant's problem is the dual of the owner's revenue
maximization problem.
ECON 2050  Optimization II
20 / 26
```

## PDF page 21

```text
A consequence of the duality theorem is that the minimum total price the entrant must pay for
the owner to accept the oer is exactly the maximum revenue that the owner can obtain from
running the bakery.
This is not too surprising:
For the owner to part with the bakery, he must receive at least as much money as it makes
by producing and selling bread and cakes.
The entrant, on the other hand, should pay no more than the revenue it could generate by
acquiring the bakery.
The story above allows us to interpret the dual variables as prices for each of the resources, or
beyond the acquisition setting, the imputed cost of using an extra unit of each of the
resources.
ECON 2050  Optimization II
21 / 26
```

## PDF page 22

```text
Another way to understand the dual is to ask: would additional resource be valuable, and if so
just how much?
The solution of the dual is (y ∗
1 , y∗
2 , y∗
3 ) = (1
2, 1
2, 0).
Note that the constraint on the fridge storage space x2 ≤6
5 is slack at the primal solution
(x∗
1, x∗
2) = (1, 1).
In other words, as long as the fridge storage space is no less than 1, the solution
(x∗
1, x∗
2) = (1, 1) is still revenue-maximizing.
Therefore, for slight changes in the fridge storage space, the value of y ∗
3 gives us the
change in optimal objective function value, namely zero.
Let's now turn to a binding constraint, say the labor constraint, and suppose the units of
available labor increases by very little, say 0.1 (so 4 becomes 4.1).
One can verify that after this change, the primal solution is still at the intersection of the
(new) labor boundary x1 + 3x2 = 4.1 and production capacity boundary x1 + x2 = 2,
which is (0.95, 1.05), and the new optimal value is 3.05 instead of 3.
But 3.05 = 3 + y ∗
1 · (change in available labor) = 3 + 0.1y ∗
1 .
ECON 2050  Optimization II
22 / 26
```

## PDF page 23

```text
To summarize, each dual variable represents the per unit increase in objective function value
from relaxing one of the primal constraints for a suciently small amount, while other things
held xed.
If each constraint of a linear program is interpreted as the restriction imposed by available
quantity of some resource, the dual variable measures the marginal value of that resource.
In other words, the dual variable is measuring the relative contribution that one unit of
that resource makes to the total economic reward or revenue.
At the optimum, the two interpretation must coincide: the marginal cost must equal to the
marginal revenue, as you learned in ECON1010 or ECON2010.
For this reason, a solution to the dual, y ∗, is called the shadow prices.
ECON 2050  Optimization II
23 / 26
```

## PDF page 24

```text
Writing down the dual
The interpretation of the dual allow us to answer the following questions regarding the dual.
1. What happens to the dual if some constraints in the primal hold with = instead of ≤(we
don't need to worry too much about ≥because it can be easily converted to ≤)?
Recall that the dual variable yi for the constraint ∑︁n
j=1 aijxj ≤bi must satisfy yi ≥0.
This is because yi can be interpreted as the marginal value of relaxing this constraint,
which cannot be negative because doing so enlarges the constraint set.
But if the constraint is ∑︁n
j=1 aijxj = bi, as bi increases the constraint set becomes
completely dierent, and therefore the marginal value can be negative.
Thus, the sign of the dual variable for a equality constraint is unconstrained.
An implication is that the dual of the linear program max{c · x : Ax = b, x ≥0} is
min y · b
s.t.
yA ≥c.
ECON 2050  Optimization II
24 / 26
```

## PDF page 25

```text
Case 1: b = 1
x1
x2
z = 1
z = 13
x1 ≤5
x1 −x2 = 1
Optimal (5, 4)
z∗= 13
Case 2: b = 3
x1
x2
z = 3
z = 9
x1 ≤5
x1 −x2 = 3
Optimal (5, 2)
z∗= 9
Maximize: z = x1 + 2x2
Subject to: x1 −x2 = b, x1, x2 ≥0, x1 ≤5
Result: b = 1 ⇒z∗= 13, but b = 3 ⇒z∗= 9
ECON 2050  Optimization II
25 / 26
```

## PDF page 26

```text
2. What happens to the dual if some variables can also take negative values?
Recall that if we interpret the variable xj as running activity j, xj ≥0 means that this
activity must be run at a non-negative level.
In this case, the dual constraint for variable xj: ∑︁m
i=1 aijyi ≥ci.
Inutuitively, this means that the marginal benet from running activity j, cj, the j-th entry
of c, must be no more than the imputed marginal cost of running this activity, ∑︁m
i=1 aijyi.
Without the nonnegativity constraint, it can't be that ∑︁m
i=1 aijyi > ci: otherwise one
would let xi →−∞to get innite prots, which makes no sense.
Thus, we should expect the dual constraint for variable xj to be ∑︁m
i=1 aijyi = ci.
An implication is that the dual of the linear program max{c · x : Ax ≤b} is
min y · b
s.t.
yA = c, y ≥0,
and the dual of the linear program max{c · x : Ax = b} is
min y · b
s.t.
yA = c.
These can be derived using the tricks on slide 7.
ECON 2050  Optimization II
26 / 26
```
