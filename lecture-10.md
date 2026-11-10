# Lecture 10: automatic text transcript

Original: [Lecture 10 PDF](lecture-10.pdf). Topic: Complementary slackness and Lagrange multipliers.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050  Mathematical Economics
Optimization III: From Linear Programming to Nonlinear Programming
ECON 2050  Optimization III
1 / 28
```

## PDF page 2

```text
Complementary slackness
Theorem
If x∗is a solution to the primal and y ∗is a solution to the dual. Then
1 y∗
i > 0 implies ∑︁
j aijx∗
j = bi;
2 ∑︁n
j=1 aijx∗
j < bi implies y ∗
i = 0;
3 x∗
j > 0 implies ∑︁m
i=1 aijy∗
i = cj;
4 ∑︁m
i=1 aijy∗
i > cj implies x∗
j = 0.
Interpretation:
1 y∗
i > 0 means that the marginal value of resource i is strictly positive, and therefore at the
optimum all the available stock of resource i must be used.
2 ∑︁n
j=1 aijx∗
j < bi means that not all available stock of resource i is used, then it must be
that the marginal value of resource i, y ∗
i , is zero.
ECON 2050  Optimization III
2 / 28
```

## PDF page 3

```text
Theorem
If x∗is a solution to the primal and y ∗is a solution to the dual. Then
1 y∗
i > 0 implies ∑︁
j aijx∗
j = bi;
2 ∑︁n
j=1 aijx∗
j < bi implies y ∗
i = 0;
3 x∗
j > 0 implies ∑︁m
i=1 aijy∗
i = cj;
4 ∑︁m
i=1 aijy∗
i > cj implies x∗
j = 0.
Interpretation (Continued): Recall from the previous lecture that cj is the marginal benet from
running activity j, and the imputed marginal cost of running activity j is ∑︁m
i=1 aijyi. Then
3 x∗
j > 0 means that the (imputed) marginal cost and marginal benet must equal, as
otherwise xj should be set to 0.
4 ∑︁m
i=1 aijy∗
i > cj means that the (imputed) marginal cost is strictly higher than marginal
benet, so engaging in activity j would incur a loss, hence x ∗
j must be zero.
ECON 2050  Optimization III
3 / 28
```

## PDF page 4

```text
Consequently, we can treat every primal constraint and its corresponding dual variable as a
complementary pair: if one is slack the other one must be binding. Thus,
y∗
i
⎛
⎝
n
∑︂
j=1
aijx∗
j −bi
⎞
⎠= 0
for every i = 1, . . . , m.
(CS1)
Similarly, we can treat every dual constraint and its corresponding primal variable as a
complementary pair: if one is slack the other one must be binding. Thus,
x∗
j
(︄m
∑︂
i=1
aijy∗
i −cj
)︄
= 0
for every j = 1, . . . , n.
(CS2)
The conditions (CS1) and (CS2) are called the complementary slackness conditions.
As we will soon see, these conditions can be very useful in solving linear or even non-linear
programming problems.
ECON 2050  Optimization III
4 / 28
```

## PDF page 5

```text
Nonlinear programming
Although linear programs are ubiquitous in economics, nance, and business, linearity of
objective or constraint functions may fail in many important problems. For example:
In a consumer's utility maximization problem, the utility function u may not be linear:
max
(x,y)∈R2 u(x, y)
s.t.
pxx + pyy ≤M
x ≥0, y ≥0
A rm whose production function is f , which may not be linear, wants to minimize costs
rK + wL while producing at least b units of output (r and w are the unit costs of the two
input factors x and y, respectively):
min
(K,L)∈R2 rK + wL
s.t.
f (K, L) ≥b
K ≥0, L ≥0
ECON 2050  Optimization III
5 / 28
```

## PDF page 6

```text
Therefore, we need to extend linear programming techniques to settings with non-linear
objective function or constraint functions.
In what follows we dene a more general problem of optimizing a (potentially non-linear)
function subject to a few (potentially non-linear) constraints, called nonlinear programming.
Let S be an open subset of Rn.
The objective function, f : S →R, is continuously dierentiable.
There are m constraint functions; for each i = 1, 2, . . . , m, gi : S →R is continuously
dierentiable.
We consider the maximization problem
max
x∈S f (x)
subject to
gi(x) ≤0 for all i = 1, . . . , m
Any non-linear program can be transformed into the above form; however, unlike linear
programs, there are pitfalls for the careless (more on that later).
ECON 2050  Optimization III
6 / 28
```

## PDF page 7

```text
Suppose x∗∈S is a solution to the non-linear program
max
x∈S f (x)
subject to
gi(x) ≤0 for all i = 1, . . . , m;
denote the constraint set by
C = {x ∈S : gi(x) ≤0 for all i = 1, . . . , m}.
Then for any x ∈C, f (x∗) ≥f (x).
Because f is continuously dierentiable, around x ∗we can approximate f by its (rst-order)
Taylor approximation (see lecture 3 slide 24):
f (x∗+ h) ≈f (x∗) + ∇f (x∗) · h.
Similarly, we can approximate each of the constraint functions gi around x∗:
gi(x∗+ h) ≈gi(x∗) + ∇gi(x∗) · h.
ECON 2050  Optimization III
7 / 28
```

## PDF page 8

```text
Because x∗maximizes f on C, the following maximization problem must have a solution h = 0:
max
h
f (x∗) + ∇f (x∗) · h
subject to
gi(x∗) + ∇gi(x∗) · h ≤0 for all i = 1, . . . , m.
Note that dropping the constant terms of the objective functions doesn't aect the solutions,
and therefore the problem above is equivalent to the following linear program:
max
h
∇f (x∗) · h
subject to
∇gi(x∗) · h ≤−gi(x∗) for all i = 1, . . . , m.
If this still doesn't seem familiar to you, let c = ∇f (x ∗),
A =
⎛
⎜
⎜
⎜
⎝
∇g1(x∗)
∇g2(x∗)
...
∇gm(x∗)
⎞
⎟
⎟
⎟
⎠,
and
b =
⎛
⎜
⎜
⎜
⎝
−g1(x∗)
−g2(x∗)
...
−gm(x∗)
⎞
⎟
⎟
⎟
⎠,
the problem can be written as max c · h subject to Ah ≤b.
ECON 2050  Optimization III
8 / 28
```

## PDF page 9

```text
The dual of the problem max c · h subject to Ah ≤b is
min λ · b
subject to
λA = c and λ ≥0.
Recalling that c = ∇f (x∗),
A =
⎛
⎜
⎜
⎜
⎝
∇g1(x∗)
∇g2(x∗)
...
∇gm(x∗)
⎞
⎟
⎟
⎟
⎠,
and
b =
⎛
⎜
⎜
⎜
⎝
−g1(x∗)
−g2(x∗)
...
−gm(x∗)
⎞
⎟
⎟
⎟
⎠,
the dual can be written as
min
λ −λ1g1(x∗) −λ2g2(x∗) −· · · −λmgm(x∗)
s.t. λ1∇g1(x∗) + λ2∇g2(x∗) + · · · + λm∇gm(x∗) = ∇f (x∗)
λi ≥0 for each i = 1, . . . , m.
ECON 2050  Optimization III
9 / 28
```

## PDF page 10

```text
Because the primal has a solution h = 0, which leads to optimal value 0. By the duality
theorem, the optimal value of the dual is also 0, implying that
−λ∗
1g1(x∗) −λ∗
2g2(x∗) −· · · −λ∗
mgm(x∗) = 0.
Because λ∗
i ≥0 and gi(x∗) ≤0, −λ∗
i gi(x∗) ≥0 for all i = 1, . . . , m. Thus, it must be that
λ∗
i gi(x∗) = 0
for all i = 1, . . . , m.
(complementary slackness)
Since the dual constraints must be satised, we see that a set of necessary conditions for x ∗
being a solution of the non-linear program is that there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0,
gi(x∗) ≤0
for all i = 1, . . . , m,
λ∗
i gi(x∗) = 0
for all i = 1, . . . , m.
These conditions are sometimes called the Langrange conditions; the dual variables λ1, . . . ,
λm are also called Lagrange multipliers.
ECON 2050  Optimization III
10 / 28
```

## PDF page 11

```text
Since the Lagrange multipliers are just dual variables, they admit the same interpretation as
what we discussed in the previous lecture.
Strictly speaking, what we obtained in the previous slide are the necessary conditions for x ∗to
be a solution of the linear approximation of the original non-linear program.
To see the only possible gap, note that the rst condition can be written as
∇f (x∗) = λ∗
1∇g1(x∗) + λ∗
2∇g2(x∗) + · · · + λ∗
m∇gm(x∗);
since λ∗
i ≥0 for all i = 1, . . . , m, the above equality means that ∇f (x ∗) is in the cone
generated by {∇g1(x∗), . . . , ∇gm(x∗)}.
As long as x∗is a solution, this is always possible for a linear program.
However, the constraint set of non-linear programs may be ill-behaved, having cusps or
pathological turning points.
Consequently, it can be that although x ∗is indeed a solution to the non-linear program,
∇f (x∗) is not in the cone generated by {∇g1(x∗), . . . , ∇gm(x∗)}.
ECON 2050  Optimization III
11 / 28
```

## PDF page 12

```text
Example: Consider the maximization problem
max
(x1,x2)∈R2 f (x1, x2) = x2
subject to
g1(x1, x2) = −x1 ≤0,
g2(x1, x2) = x1 + x2
2 ≤0.
The only point in R2 that satises the constraints is (0, 0); so (0, 0) must be the unique
solution.
O
x1
x2
x1 + x2
2 = 0
∇f (0, 0)
∇g2(0, 0)
∇g1(0, 0)
Now ∇f (0, 0) = (0, 1), ∇g1(0, 0) = (−1, 0), and ∇g2(0, 0) = (1, 0).
Observe that ∇f (0, 0) is not in the cone generated by {∇g1(0, 0), ∇g2(0, 0)}
Therefore we can't nd λ1, λ2 ≥0 such that ∇f (0, 0) = λ1∇g1(0, 0) + λ2∇g2(0, 0)
Lagrange conditions are not necessary in that they're not satised by the unique solution
ECON 2050  Optimization III
12 / 28
```

## PDF page 13

```text
Necessary conditions
Thankfully, when the constraint functions are all ane (like in a linear program, although the
objective function can be non-linear), we don't have to worry:
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable function, and
each gj : S →R, j = 1, . . . , m, is an ane function. If x∗∈S and it is a solution to problem
max
x∈S f (x)
s.t. gi(x) ≤0 for i = 1, . . . , m,
then there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0,
gi(x∗) ≤0
for all i = 1, . . . , m,
λ∗
i gi(x∗) = 0
for all i = 1, . . . , m.
ECON 2050  Optimization III
13 / 28
```

## PDF page 14

```text
The condition ∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0 can also be
obtained through an auxiliary function called the Lagrangian:
L(x, λ) = f (x) −λ1g1(x) −λ2g2(x) −· · · −λmgm(x).
If x∗∈S is a solution to the non-linear program, then there exists a λ∗≥0 such that
∂L(x∗, λ∗)
∂x1
= ∂f (x∗)
∂x1
−λ∗
1
∂g1(x∗)
∂x1
−· · · −λ∗
m
∂gm(x∗)
∂x1
= 0,
∂L(x∗, λ∗)
∂x2
= ∂f (x∗)
∂x2
−λ∗
1
∂g1(x∗)
∂x2
−· · · −λ∗
m
∂gm(x∗)
∂x2
= 0,
...
∂L(x∗, λ∗)
∂xn
= ∂f (x∗)
∂xn
−λ∗
1
∂g1(x∗)
∂xn
−· · · −λ∗
m
∂gm(x∗)
∂xn
= 0.
Therefore, the solution x∗can be interpreted as a critical point of L(x, λ∗), where the
rst-order conditions hold (but don't forget the constraints themselves, gi(x∗) ≤0, and
complementary slackness, λ∗
i gi(x∗) = 0).
ECON 2050  Optimization III
14 / 28
```

## PDF page 15

```text
If some of the constraint functions are not ane, as long as the set of gradients of constraint
functions binding at x∗is linearly independent, we also have no trouble:
Theorem
Let S be an open subset of Rn, and let f : S →R and gj : S →R, j = 1, . . . , m be
continuously dierentiable functions. Suppose x ∗∈S is a solution to the problem
max
x∈S f (x)
s.t. gi(x) ≤0 for i = 1, . . . , m,
and suppose the rst k ≤m constraints are binding, and the other m −k constraints are slack.
If the set of gradients of the binding constraints, {∇g1(x∗), . . . , ∇gk(x∗)}, is linearly
independent, then there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0,
gi(x∗) ≤0
for all i = 1, . . . , m,
λ∗
i gi(x∗) = 0
for all i = 1, . . . , m.
ECON 2050  Optimization III
15 / 28
```

## PDF page 16

```text
The trickiness with the linear independence test is that we can't determine which constraints
are binding until we have identied candidate solutions from the Lagrange conditions.
What we usually do instead is to test the linear independence of the set of gradients of all
constraint functions, {∇g1(x), . . . , ∇gm(x)}, before writing down the Lagrange conditions
If the set {∇g1(x), . . . , ∇gm(x)} is linearly independent for every x in the constraint set,
then we're completely safe.
If not, things become more complicated, but in simple problems the number of points y in
the constraint set such that {∇g1(y), . . . , ∇gm(y)} is linearly dependent is usually small.
When there are a small number of constraints, we can check what happens when each of
the subsets of the constraints bind (more on that in the next lecture).
ECON 2050  Optimization III
16 / 28
```

## PDF page 17

```text
Example: Consider the maximization problem
max
(x1,x2)∈R2 x2
1 + x2
2
s.t.
x1 + x2 −1 ≥0.
To apply the theorem, we rst need to write the constraint as g(x1, x2) ≡1 −x1 −x2 ≤0.
One way to see that the Lagrange conditions are necessary is that the lone constraint
function is ane. One can also note that ∇g(x1, x2) = (1, 1) ̸= (0, 0) for all (x1, x2) ∈R2,
and hence {∇g(x1, x2)} is linearly independent for every (x1, x2) in the constraint set.
The Lagrange conditions are
2x1 + λ = 0
2x2 + λ = 0
λ(1 −x1 −x2) = 0
λ ≥0
1 −x1 −x2 ≤0
ECON 2050  Optimization III
17 / 28
```

## PDF page 18

```text
Rule of thumb: The most convenient way of solving the Lagrange conditions is usually to start
from complementary slackness.
If λ = 0, then from the rst two equalities we see that x1 = x2 = 0, violating
1 −x1 −x2 ≤0. Thus, λ > 0.
Consequently, complementary slackness requires x1 + x2 = 1.
From the rst two equalities (2x1 + λ = 0 and 2x2 + λ = 0), we see that x1 = x2 = −λ/2.
Together with x1 + x2 = 1, we get x1 = x2 = 1/2 and λ = −1. But λ > 0, a contradiction.
Thus, there is no point that satises the Lagrange conditions for this problem.
Because the Lagrange conditions are necessary, that is, every solution must satisfy the
Lagrange conditions, the maximization problem has no solution.
ECON 2050  Optimization III
18 / 28
```

## PDF page 19

```text
Graphically:
−0.5
0.5
1
1.5
2
2.5
3
−0.5
0.5
1
1.5
2
2.5
3
f →∞
Constraint
Set
x1
x2
ECON 2050  Optimization III
19 / 28
```

## PDF page 20

```text
If we can use the extreme value theorem to conclude that a solution exists, we have a useful
cookbook procedure for solving non-linear programs:
We rst check if all constraint functions are ane. If so,
Write down the Langrange conditions.
Every x that (together with some λ) satises the Lagrange conditions is a candidate
solution.
The candidates at which the value of the objective function are the largest are the
solutions.
If not:
Check whether the set of gradients of the constraint functions is linearly independent;
identify the points at which it is not.
Write down the Langrange conditions.
Every x that violates the linear independence condition or that (together with some λ)
satises the Lagrange conditions is a candidate solution.
The candidates at which the value of the objective function are the largest are the
solutions.
ECON 2050  Optimization III
20 / 28
```

## PDF page 21

```text
Exercise: Solve the maximization problem
max
(x,y)∈R2 f (x, y) = x + y
s.t.
g(x, y) = x2 + y2 −2 ≤0.
By the extreme value theorem, the maximization problem has a solution.
Since ∇g(x, y) = (2x, 2y) = (0, 0) only if (x, y) = (0, 0), {∇g(x, y)} is linearly
independent for every (x, y) in the constraint set except for (0, 0).
However, (0, 0) doesn't make the constraint bind, and therefore the set of gradients of the
binding constraints is always linearly independent.
Thus, the Lagrange conditions are necessary; i.e., every solution of this problem must
satisfy the Lagrange conditions.
ECON 2050  Optimization III
21 / 28
```

## PDF page 22

```text
The Lagrange conditions are
1 −2λx = 0
(1)
1 −2λy = 0
(2)
λ(x2 + y2 −2) = 0
(3)
x2 + y2 ≤2
(4)
λ ≥0
(5)
If λ = 0 then neither (1) nor (2) are satised. Hence λ > 0 and, by the complementary
slackness condition (3), x2 + y2 = 2.
(1) and (2) then imply x = y; plugging it into x 2 + y2 = 2, either x = y = 1 or
x = y = −1.
But if x = y = −1, (1) or (2) implies that λ = −1/2, a contradiction.
Thus, only point that satises the Lagrange conditions is (x ∗, y∗, λ∗) = (1, 1, 1/2).
Then since a solution exists, and every solution must satisfy the Lagrange conditions, the
unique solution is (x∗, y∗) = (1, 1).
ECON 2050  Optimization III
22 / 28
```

## PDF page 23

```text
Equality constraints
On slide 6, we mentioned that every constraint can be written as a less than or equal to
constraint. Specically,
If the constraint looks like g(x) ≤h(x), we can write it as g(x) −h(x) ≤0.
gi(x) ≥0 can be written as −gi(x) ≤0.
gi(x) = 0 can be replaced by two inequality constraints: gi(x) ≤0 and −gi(x) ≤0.
If all constraint functions are ane, everything works out smoothly. However, if not, we need
to test linear independence of the set of gradients of the binding constraint functions.
The linear independence of that set is sensitive to the representation of the constraint set.
To see why, consider the problem max f (x) subject to g(x) = 0.
This can be written as max f (x) subject to g(x) ≤0 and −g(x) ≤0.
However, both constraints bind, and the set of gradients {∇g(x), −∇g(x)} is linearly
dependent, and therefore we can't use the theorem on slide 15.
ECON 2050  Optimization III
23 / 28
```

## PDF page 24

```text
Thankfully, the power of the duality theorem allows us to handle equality constraints easily.
The linear program on slide 8 now becomes, replacing ≤by =,
max
h
∇f (x∗) · h
subject to
∇gi(x∗) · h = −gi(x∗) for all i = 1, . . . , m.
Its dual is
min
λ −λ1g1(x∗) −λ2g2(x∗) −· · · −λmgm(x∗)
s.t. λ1∇g1(x∗) + λ2∇g2(x∗) + · · · + λm∇gm(x∗) = ∇f (x∗)
The only dierence is that the sign of the dual variables (Lagrange multipliers) are unrestricted.
Because the constraints are equalities rather than inequalities, complementary slackness is
no longer meaningful.
ECON 2050  Optimization III
24 / 28
```

## PDF page 25

```text
The discussion in the previous two slides gives rise to the following result:
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable function.
Suppose
either each gj : S →R, j = 1, . . . , m, is an ane function,
or each gj : S →R, j = 1, . . . , m, is continuously dierentiable, and the set of gradients of
constraint functions {g1(x∗), . . . , gm(x∗)} is linearly independent.
If x∗∈S and it is a solution to problem
max
x∈S f (x)
s.t. gi(x) = 0 for i = 1, . . . , m,
Then there exists λ∗= (λ∗
1, . . . , λ∗
m) ∈Rm such that gi(x∗) = 0 for each i = 1, . . . , m, and
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0.
ECON 2050  Optimization III
25 / 28
```

## PDF page 26

```text
When the constraints are equalities, there is an even closer analogy between the rst-order
conditions and the Lagrange conditions. To see this, consider again the Lagrangian:
L(x, λ) = f (x) −λ1g1(x) −λ2g2(x) −· · · −λmgm(x).
If x∗∈S is a solution to the non-linear program with equality constraints, there exists
λ∗∈Rm:
∂L(x∗, λ∗)
∂x1
= ∂f (x∗)
∂x1
−λ∗
1
∂g1(x∗)
∂x1
−· · · −λ∗
m
∂gm(x∗)
∂x1
= 0,
...
∂L(x∗, λ∗)
∂xn
= ∂f (x∗)
∂xn
−λ∗
1
∂g1(x∗)
∂xn
−· · · −λ∗
m
∂gm(x∗)
∂xn
= 0,
∂L(x∗, λ∗)
∂λ1
= g1(x∗) = 0,
· · · ,
∂L(x∗, λ∗)
∂λm
= gm(x∗) = 0.
Therefore, if x∗is a solution, (x∗, λ∗) is a critical point of L(x, λ), where the rst-order
conditions hold.
ECON 2050  Optimization III
26 / 28
```

## PDF page 27

```text
Example: Consider the maximization problem
max
(x1,x2)∈R2 f (x1, x2) = −2x2
1 −3x2
2
s.t.
g(x1, x2) = x1 + x2 −1 = 0.
We can either use the fact that g is ane, or to notice that ∇g(x1, x2) = (1, 1) ̸= (0, 0)
for all (x1, x2) ∈R2, and therefore {∇g(x1, x2)} is linearly independent for every (x, y) in
the constraint set, to conclude that the Lagrange conditions are necessary.
The Lagrange conditions are
−4x1 + λ = 0
−6x2 + λ = 0
x1 + x2 −1 = 0
From the rst two equations we get λ = 4x1 = 6x2, and therefore x1 = 3
2x2.
Plugging into the third equation (the equality constraint), we get the unique solution
(x∗
1, x∗
2, λ∗) = (3/5, 2/5, 12/5).
Because the extreme value theorem fails to hold (why?), we can only claim that if this
problem has a solution, then it must be (x ∗
1, x∗
2) = (3/5, 2/5).
ECON 2050  Optimization III
27 / 28
```

## PDF page 28

```text
A more general result for problems with both equality and inequality constraints:
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable function.
Suppose
either each gj : S →R, j = 1, . . . , m, is an ane function,
or each gj : S →R, j = 1, . . . , m, is continuously dierentiable, and the set of gradients of
constraint functions binding at x ∗is linearly independent.
If x∗∈S and it is a solution to problem
max
x∈S f (x)
s.t. gi(x) = 0 for i = 1, . . . , k, and gi(x) ≤0 for i = k + 1, . . . , m,
Then there exists λ∗= (λ∗
1, . . . , λ∗
m) ∈Rm such that λi ≥0 for each i = k + 1, . . . , m, and
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) = 0,
gi(x∗) = 0 for all i = 1, . . . , k, and gi(x∗) ≤0 for all i = k + 1, . . . , m,
λ∗
i gi(x∗) = 0
for all i = k + 1, . . . , m.
ECON 2050  Optimization III
28 / 28
```
