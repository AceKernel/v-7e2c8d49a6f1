# Lecture 11: automatic text transcript

Original: [Lecture 11 PDF](lecture-11.pdf). Topic: KKT and sufficiency.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050  Mathematical Economics
Optimization IV: Nonlinear Programming, Endgame
ECON 2050  Optimization IV
1 / 25
```

## PDF page 2

```text
A (particularly relevant) special class of problems
In economics, nance, and business, we commonly work with nonnegative variables such as
quantities and prices. Therefore, we often have to solve problems of the form
max
x∈S f (x)
s.t.
g1(x) ≤0, . . . , gm(x) ≤0
(♢)
x1 ≥0, . . . , xn ≥0
(1)
where S ⊆Rn is open and f , g1, . . . , gm : S →R are continuously dierentiable.
Problems of this form are so ubiquitous that, although we can tackle them with our previous
theorem on inequality constraints, a special theorem has been derived for them.
ECON 2050  Optimization IV
2 / 25
```

## PDF page 3

```text
To start with, consider a constrained maximization problem
max
(x1,x2)∈R2 f (x1, x2)
subject to
g(x1, x2) ≤0, x1 ≥0, x2 ≥0.
We could let n1(x1, x2) = −x1 and n2(x1, x2) = −x2, and the problem becomes
max
(x1,x2)∈R2 f (x1, x2)
subject to
g(x1, x2) ≤0, n1(x1, x2) ≤0, n2(x1, x2) ≤0.
The Lagrange conditions for this problem are
∂f (x1, x2)
∂x1
−λ∂g(x1, x2)
∂x1
+ ν1 = 0
∂f (x1, x2)
∂x2
−λ∂g(x1, x2)
∂x2
+ ν2 = 0
g(x1, x2) ≤0, λ ≥0, x1 ≥0, x2 ≥0
λg(x1, x2) = 0, ν1x1 = 0, ν2x2 = 0
ECON 2050  Optimization IV
3 / 25
```

## PDF page 4

```text
The rst two equalities can be written as
∂f (x1, x2)
∂x1
−λ∂g(x1, x2)
∂x1
= −ν1,
∂f (x1, x2)
∂x2
−λ∂g(x1, x2)
∂x2
= −ν2
(△)
Since ν1, ν2 ≥0, (△) is equivalent to
∂f (x1, x2)
∂x1
−λ∂g(x1, x2)
∂x1
≤0
∂f (x1, x2)
∂x2
−λ∂g(x1, x2)
∂x2
≤0
⇐⇒
∇f (x1, x2) −λ∇g(x1, x2) ≤0.
Again by (△), the two complementary slackness conditions, ν1x1 = 0 and ν2x2 = 0, become
x1
(︃∂f (x1, x2)
∂x1
−λ∂g(x1, x2)
∂x1
)︃
= 0
and
x2
(︃∂f (x1, x2)
∂x2
−λ∂g(x1, x2)
∂x2
)︃
= 0
Bringing back the other four conditions, g(x1, x2) ≤0, λ ≥0, x1 ≥0, x2 ≥0, and
λg(x1, x2) = 0, we obtained a new set of conditions without the Lagrange multipliers on the
nonnegativity constraints, ν1 and ν2.
ECON 2050  Optimization IV
4 / 25
```

## PDF page 5

```text
Karush-Kuhn-Tucker (KKT) conditions
Going back to the more general maximization problem (♢), we see that a set of necessary
conditions for x∗≥0 being a solution to the non-linear program with non-negative variables is
that there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) ≤0,
x∗
i
(︃∂f (x∗)
∂xi
−λ∗
1
∂g1(x∗)
∂xi
−λ∗
2
∂g2(x∗)
∂xi
−· · · −λ∗
m
∂gm(x∗)
∂xi
)︃
= 0
for all i = 1, . . . , n,
gj(x∗) ≤0
for all j = 1, . . . , m,
λ∗
j gj(x∗) = 0
for all j = 1, . . . , m.
These conditions are sometimes called the Karush-Kuhn-Tucker (KKT) conditions.
ECON 2050  Optimization IV
5 / 25
```

## PDF page 6

```text
Alternatively, one can also set up the Lagrangian without considering the nonnegativity
constraints:
˜L(x, λ) = f (x) −λ1g1(x) −λ2g2(x) −· · · −λmgm(x),
and the KKT conditions can be expressed in the following equivalent way: if x ∗≥0 is a
solution to the non-linear program with non-negative variables, then there exists
λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∂˜L(x∗, λ∗)
∂x1
≤0, . . . , ∂˜L(x∗, λ∗)
∂xn
≤0,
(2)
x∗
1
∂˜L(x∗, λ∗)
∂x1
= 0, . . . , x∗
n
∂˜L(x∗, λ∗)
∂xn
= 0,
(3)
∂˜L(x∗, λ∗)
∂λ1
≥0, . . . , ∂˜L(x∗, λ∗)
∂λm
≥0,
(4)
λ∗
1
∂˜L(x∗, λ∗)
∂λ1
= 0, . . . , λ∗
m
∂˜L(x∗, λ∗)
∂λm
= 0.
(5)
ECON 2050  Optimization IV
6 / 25
```

## PDF page 7

```text
Theorem
Let S be an open subset of Rn, and let f : S →R be continuously dierentiable functions.
Suppose
either each gj : S →R, j = 1, . . . , m, is an ane function,
or each gj : S →R, j = 1, . . . , m, is continuously dierentiable, and the set of gradients of
constraint functions (including the nonnegative constraints) binding at x ∗is linearly
independent.
If x∗∈S and it is a solution to problem
max
x∈S f (x)
s.t. gj(x) ≤0 for j = 1, . . . , m, and x ≥0.
Then there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that (x∗, λ∗) satises the Karush-Kuhn-Tucker
(KKT) conditions.
ECON 2050  Optimization IV
7 / 25
```

## PDF page 8

```text
Example: Let u(x1, x2) be the utility function of a consumer, where x1 and x2 are the quantity
of goods 1 and 2, respectively. For each i = 1, 2, pi > 0 is the price of good i, and w > 0 is
the consumer's wealth or income. The consumer's consumption choice problem is
max
(x1,x2)∈Rn
u(x1, x2)
s.t.
p1x1 + p2x2 ≤w
xk ≥0 for k = 1, 2.
and the KKT conditions are
∂u(x1, x2)
∂x1
−λp1 ≤0,
x1
(︃∂u(x1, x2)
∂x1
−λp1
)︃
= 0,
x1 ≥0,
∂u(x1, x2)
∂x2
−λp2 ≤0,
x2
(︃∂u(x1, x2)
∂x2
−λp2
)︃
= 0,
x2 ≥0,
p1x1 + p2x2 −w ≤0,
λ(p1x1 + p2x2 −w) = 0,
λ ≥0.
ECON 2050  Optimization IV
8 / 25
```

## PDF page 9

```text
If we can use the extreme value theorem to conclude that a solution exists, similar to the
previous lecture, we have a useful cookbook procedure for solving non-linear programs with
non-negative variables:
We rst check if all constraint functions are ane. If so,
Write down the KKT conditions.
Every x that (together with some λ) satises the KKT conditions is a candidate solution.
The candidates at which the value of the objective function are the largest are the
solutions.
If not:
Check whether the set of gradients of the constraint functions is linearly independent;
identify the points at which it is not (note that the non-negativity constraints x ≥0 also
need to be considered).
Write down the KKT conditions.
Every x that violates the linear independence condition or that (together with some λ)
satises the KKT conditions is a candidate solution.
The candidates at which the value of the objective function are the largest are the
solutions.
ECON 2050  Optimization IV
9 / 25
```

## PDF page 10

```text
Example: Consider the maximization problem
max
(x1,x2)∈R2
x1x2
s.t.
x1 + x2 ≤6
x1 ≥0,
x2 ≥0.
Observe that the constraint functions are ane, so the KKT conditions are necessary; that
is, every solution of the maximization problem must satisfy the KKT conditions.
The KKT conditions are
x2 −λ ≤0,
x1(x2 −λ) = 0,
x1 ≥0,
x1 −λ ≤0,
x2(x1 −λ) = 0,
x2 ≥0,
x1 + x2 −6 ≤0,
λ(x1 + x2 −6) = 0,
λ ≥0.
If x1 > 0, since x1(x2 −λ) = 0, we must have x2 = λ. If x2 = λ = 0, then x1 −λ ≤0
implies that x1 ≤0, a contradiction. Thus, x2 > 0.
But then x2(x1 −λ) = 0 implies that x1 = λ = x2 > 0.
ECON 2050  Optimization IV
10 / 25
```

## PDF page 11

```text
Because λ > 0, by complementary slackness, 6 −x1 −x2 = 0. Therefore,
(x∗
1, x∗
2, λ∗) = (3, 3, 3) satises the KKT conditions.
Now suppose instead x1 = 0. If x2 > 0, by complementary slackness, x2(x1 −λ) = 0
implies λ = x1 = 0.
But then since x2 −λ ≤0, it must be that x2 ≤0, a contradiction. Thus, x∗
2 = λ∗= 0.
Therefore, (x∗
1, x∗
2, λ∗) = (0, 0, 0) also satises the KKT conditions.
Because the objective function is continuous and the constraint set is compact (draw a
picture), by the extreme value theorem a solution exists.
Then since the KKT conditions are necessary, all solutions must be among the points at
which the KKT conditions are satised.
Because the value of the objective function at (x1, x2) = (3, 3) is strictly greater than that
at (0, 0), the unique solution of the problem is (x ∗
1, x∗
2) = (3, 3).
ECON 2050  Optimization IV
11 / 25
```

## PDF page 12

```text
Exercise: Consider the maximization problem
max f (x, y) = x + y
s.t.
x2 + y2 ≤2, x ≥0, y ≥0
Denote the three constraint functions by g(x, y) = x 2 + y2 −2, n1(x, y) = −x,
n2(x, y) = −y.
The linear independence condition is satised at all relevant points:
▶If exactly 1 constraint binds, the corresponding gradient is non-zero:
⋆If x = 0 is the only binding constraint, since ∇n1(x, y) = (−1, 0), the set of gradients of binding
constraint functions is {(−1, 0)}, which is linearly independent.
⋆If y = 0 is the only binding constraint, since ∇n2(x, y) = (0, −1), the set of gradients of binding
constraint functions is {(0, −1)}, which is linearly independent.
⋆If x2 + y 2 = 2 is the binding constraint, since ∇g(x, y) = (2x, 2y), it is only zero when
(x, y) = (0, 0), but the constraint doesn't bind at this point. Thus, {∇g(x, y)} is linearly
independent when g(x, y) ≤0 is binding.
ECON 2050  Optimization IV
12 / 25
```

## PDF page 13

```text
The linear independence condition is satised at all relevant points:
▶If exactly 2 constraints bind, then the set of gradients of binding constraint functions is
always linearly independent:
⋆If x = 0 and y = 0, since ∇n1(x, y) = (−1, 0) and ∇n2(x, y) = (0, −1) the set of gradients of
binding constraint functions is
{(−1, 0), (0, −1)} , which is linearly independent
⋆If x = 0 and x2 + y 2 = 2 then y =
√
2 and since ∇g(x, y) = (2x, 2y) and ∇n1(x, y) = (−1, 0),
the set of gradients of constraint functions binding at (x, y) = (0,
√
2) is
{∇g(0,
√
2), ∇n1(0,
√
2)} = {(0, 2
√
2), (−1, 0)},
which is linearly independent.
⋆If y = 0 and x2 + y 2 = 2 then x =
√
2 ∇g(x, y) = (2x, 2y) and ∇n2(x, y) = (0, −1),
the set of gradients of constraint functions binding at (x, y) = (
√
2, 0) is
{∇g(
√
2, 0), ∇n2(
√
2, 0)} = {(2
√
2, 0), (0, −1)},
which is linearly independent.
▶It is not possible that all 3 constraints bind: x = y = 0 implies x 2 + y 2 < 2.
ECON 2050  Optimization IV
13 / 25
```

## PDF page 14

```text
KKT conditions: x ≥0, y ≥0, λ ≥0,
1 −2λx ≤0
(6)
x(1 −2λx) = 0
(7)
1 −2λy ≤0
(8)
y(1 −2λy) = 0
(9)
x2 + y2 ≤2,
(10)
λ(x2 + y2 −2) = 0
(11)
From (6) and (8) we infer that λ > 0, x > 0, y > 0. Therefore,
1 −2λx = 0,
1 −2λy = 0,
x2 + y2 = 2.
We obtain the unique point that satises KKT: (x ∗, y∗, λ∗) = (1, 1, 1
2).
Since the constraint set is compact and the objective function is continuous, (1, 1) is the
unique solution (extreme value theorem).
ECON 2050  Optimization IV
14 / 25
```

## PDF page 15

```text
Sucient conditions
In lecture 8, we saw that when the objective function is concave, the rst-order conditions
become sucient; i.e., every critical point is an optimal solution.
Since the Lagrange/KKT conditions admit a similar interpretation to the rst-order conditions,
it's natural to expect that a similar result should hold here.
Indeed, under further assumptions on the constraint functions, we could obtain such
suciency results.
The rough idea of these conditions is that they guarantee that the constraint set is convex,
implying that the concave objective function is well dened, and that local optimality
implies global optimality.
ECON 2050  Optimization IV
15 / 25
```

## PDF page 16

```text
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable concave
function, and each gj : S →R, j = 1, . . . , m, is a continuously dierentiable convex function.
If x∗∈S and there exists λ∗= (λ∗
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
for all i = 1, . . . , m,
then x∗is a solution to problem
max
x∈S f (x)
s.t. gi(x) ≤0 for i = 1, . . . , m.
ECON 2050  Optimization IV
16 / 25
```

## PDF page 17

```text
Proof: Denote the constraint set by C ≡{x ∈S : gi(x) ≤0 for i = 1, . . . , m}.
Recall the alternative interpretation of the rst equality in the Lagrange conditions: it is the
rst-order condition of the Lagrangian
L(x, λ∗) = f (x) −λ∗
1g1(x) −λ∗
2g2(x) −· · · −λ∗
mgm(x).
Note that we are taking λ∗= (λ∗
1, . . . , λ∗
m) as constants here so L is only a function of x.
Because for each i = 1, . . . , m, gi is convex, −gi is concave. Therefore, L, as the sum of
concave functions, is also concave. Consequently, since x ∗is a critical point of L, it maximizes
L on S.
Since C ⊆S, x∗also maximizes L on C, meaning that L(x ∗, λ∗) ≥L(x, λ∗) for all x ∈C.
Then
f (x∗) = L(x∗, λ∗) ≥L(x, λ∗) ≥f (x)
for all x ∈C, where the equality follows from complementary slackness (which implies that
λ∗
1g1(x∗) −λ∗
2g2(x∗) −· · · −λ∗
mgm(x∗) = 0), and the second inequality holds because λ∗
i ≥0
and gi(x) ≤0 for each i = 1, . . . , m. Thus, x∗is a solution to the maximization problem.
ECON 2050  Optimization IV
17 / 25
```

## PDF page 18

```text
An analogous result can be obtained for points satisfying the KKT conditions.
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable concave
function, and each gj : S →R, j = 1, . . . , m, is a continuously dierentiable convex function.
If x∗∈S and there exists λ∗= (λ∗
1, . . . , λ∗
m) ≥0 such that
∇f (x∗) −λ∗
1∇g1(x∗) −λ∗
2∇g2(x∗) −· · · −λ∗
m∇gm(x∗) ≤0,
x∗
i
(︃∂g1(x∗)
∂xi
−λ∗
2
∂g2(x∗)
∂xi
−· · · −λ∗
m
∂gm(x∗)
∂xi
)︃
= 0
for all i = 1, . . . , n,
gj(x∗) ≤0
for all j = 1, . . . , m,
λ∗
j gj(x∗) = 0
for all j = 1, . . . , m,
then x∗is a solution to problem
max
x∈S f (x)
s.t. gi(x) ≤0 for i = 1, . . . , m, and x ≥0.
ECON 2050  Optimization IV
18 / 25
```

## PDF page 19

```text
Example: We saw from the exercise on slide 12 that for the maximization problem
max f (x, y) = x + y
s.t.
x2 + y2 ≤2, x ≥0, y ≥0,
the only point that satises the KKT conditions is (x ∗, y∗) = (1, 1).
To conclude that (1, 1) is indeed a solution, we can
either apply the extreme value theorem like what we did in the exercise,
or note that the objective function is concave and the constraint function
g(x, y) = x2 + y2 −2 is convex, and then apply the theorem on the previous slide.
ECON 2050  Optimization IV
19 / 25
```

## PDF page 20

```text
With equality constraints, we need to further assume that the constraint functions are ane.
Otherwise, the constraint set need not be convex.
Theorem
Let S be an open subset of Rn, and let f : S →R be a continuously dierentiable concave
function, and each gj : S →R, j = 1, . . . , m, is an ane function.
If x∗∈S and there exists λ∗= (λ∗
1, . . . , λ∗
m) ∈Rm such that gi(x∗) = 0 for each i = 1, . . . , m,
and
∇f (x∗) −λ1∇g1(x∗) −λ2∇g2(x∗) −· · · −λm∇gm(x∗) = 0,
then x∗is a solution to problem
max
x∈S f (x)
s.t. gi(x) = 0 for i = 1, . . . , m.
ECON 2050  Optimization IV
20 / 25
```

## PDF page 21

```text
Example: Let's revisit a maximization problem we saw in the previous lecture:
max
(x1,x2)∈R2 f (x1, x2) = −2x2
1 −3x2
2
s.t.
g(x1, x2) = x1 + x2 −1 = 0.
Since the constraint functions are ane, we know that every solution satises the
Lagrange conditions.
Because the objective function f is concave and the constraint function g is ane, every
point satisfying the Lagrange conditions is a solution.
In the previous lecture, we identied the unique point satisfying the Lagrange conditions:
(x∗
1, x∗
2, λ∗) = (3/5, 2/5, 12/5).
Thus, the unique solution is (x∗
1, x∗
2) = (3/5, 2/5).
ECON 2050  Optimization IV
21 / 25
```

## PDF page 22

```text
The example on the previous slide reveals a much more general feature:
Corollary
Let S be an open subset of Rn, and suppose f : S →R be a continuously dierentiable
concave function, and each gj : S →R, j = 1, . . . , m, is an ane function. Then
x∗is a solution to the constrained optimization problem with equality constraints if and
only if there exists λ∗∈Rm such that (x∗, λ∗) satises the corresponding Lagrange
conditions;
x∗is a solution to the constrained optimization problem with inequality constraints if and
only if there exists λ∗≥0 such that (x∗, λ∗) satises the corresponding Lagrange
conditions;
x∗is a solution to the constrained optimization problem with inequality constraints and
nonnegativity constraints if and only if there exists λ∗≥0 such that (x∗, λ∗) satises the
corresponding KKT conditions.
That is, the set of points satisfy the Lagrange/KKT conditions coincide with the set of
solutions of the constrained optimization problem.
ECON 2050  Optimization IV
22 / 25
```

## PDF page 23

```text
Consider a linear programming problem max{c · x : Ax ≤b, x ≥0}. To be more concrete, let
c = (c1, c2),
A =
(︃a11
a12
a21
a22
)︃
,
and
b = (b1, b2);
that is, the problem can be written as
max
(x1,x2)∈R2 c1x1 + c2x2
s.t.
a11x1 + a12x2 ≤b1
a21x1 + a22x2 ≤b2
x1 ≥0, x2 ≥0
Its dual is min{y · b : yA ≥c, y ≥0}, which can be written as
min
(y1,y2)∈R2 b1y1 + b2y2
s.t.
a11y1 + a21y2 ≥c1
a12y1 + a22y2 ≥c2
y1 ≥0, y2 ≥0
ECON 2050  Optimization IV
23 / 25
```

## PDF page 24

```text
KKT for linear programming problems
By the result on slide 22, since the objective function is linear and therefore concave, the
solutions of this problem are precisely the points satisfying the KKT conditions.
The KKT conditions are
c1 −λ1a11 −λ2a21 ≤0,
x1(c1 −λ1a11 −λ2a21) = 0,
x1 ≥0;
c2 −λ1a12 −λ2a22 ≤0,
x2(c2 −λ1a12 −λ2a22) = 0,
x2 ≥0;
a11x1 + a12x2 −b1 ≤0,
λ1(a11x1 + a12x2 −b1) = 0,
λ1 ≥0;
a21x1 + a22x2 −b2 ≤0,
λ2(a21x1 + a22x2 −b2) = 0,
λ2 ≥0.
Observe that (by changing λ1, λ2 to y1, y2) the KKT conditions are precisely the dual
constraints, primal constraints, and the complementary slackness conditions.
ECON 2050  Optimization IV
24 / 25
```

## PDF page 25

```text
This exercise further elucidates the essence of the Lagrange/KKT approach:
We write down all the primal constraints, dual constraints, and complementary slackness
conditions; these are called Lagrange/KKT conditions.
We know from our previous discussion that these must be satised by any pair of primal
solution and dual solution, (x ∗, y ∗) (when the constraint functions are not ane, further
technical assumptions needed to guarantee that the dual constraints make sense).
Therefore, by checking which points satisfy the Lagrange/KKT conditions, we rule out
most points in the constraint set; that is, we use these conditions to screen irrelevant
points.
Then by comparing the objective function's values at (usually small amount of) surviving
points, we obtain the solutions.
In particular, if the objective function is concave and the constraint functions are ane,
solving Lagrange/KKT conditions directly yield the solutions of the maximization problem.
ECON 2050  Optimization IV
25 / 25
```
