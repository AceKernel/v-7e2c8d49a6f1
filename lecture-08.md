# Lecture 8: automatic text transcript

Original: [Lecture 8 PDF](lecture-08.pdf). Topic: Unconstrained optimisation and existence.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050  Mathematical Economics
Optimization I: Basics
ECON 2050  Optimization I
1 / 25
```

## PDF page 2

```text
Optimization problems
We are now in a position to deal with optimization problems!
In this course, we focus on optimization problems that the values of a given function f : S →R
are to be maximized or minimized over a set D, where D ⊆S ⊆Rn.
Call the function f the objective function, and the set D is called the constraint set.
We can describe a maximization problem as follows:
maximize f (x)
subject to x ∈D;
or more compactly, maxx∈D f (x). A minimization problem can be described analogously.
A solution to a maximization [minimization] problem is a point x ∈D such that f (x) ≥f (y)
[f (x) ≤f (y)] for all y ∈D.
ECON 2050  Optimization I
2 / 25
```

## PDF page 3

```text
As the following examples point out, in a given maximization problem, a solution may fail to
exist; even if a solution exists, it need not be unique.
Example: Let D = R+ and f : R →R be dened by f (x) = x. Consider the maximization
problem maxx∈D f (x): we have f (D) ≡{y ∈R : y = f (x) for some x ∈D} = R+, meaning
that f (x) →∞as x →∞, so this maximization problem has no solution.
Example: Let E = [0, 1). Consider the maximization problem maxx∈E f (x), we have
f (E) = [0, 1). This means that the as x approaches 1, f (x) get closer and closer to 1
but never reaches 1 since 1 /∈E. Thus, this maximization problem has no solution.
Example: Let C = [−1, 1] and g : R →R be dened by g(x) = x2. By drawing a picture, we
see that the maximization problem maxx∈C g(x) has two solutions: x = −1 and x = 1.
ECON 2050  Optimization I
3 / 25
```

## PDF page 4

```text
Local and global extrema
Denition
Let D ⊆Rn and f : D →R. We say that x∗∈D is a
(global) maximum [minimum] of f if f (x ∗) ≥[≤] f (x), ∀x ∈D.
(global) extremum of f if x∗is a (global) minimum or a (global) maximum of f .
local maximum [minimum] of f if there exists an open ball Br(x∗) such that
f (x∗) ≥[≤] f (x), ∀x ∈Br(x∗) ∩D.
local extremum of f if x∗is a local minimum or a local maximum of f .
Every (global) maximum [minimum] is a local maximum [minimum], but the converse is false.
ECON 2050  Optimization I
4 / 25
```

## PDF page 5

```text
Example: The function f : [−3, 3] × [−3, 3] →R with the graph depicted below has 1 global
maximum, (at least) 3 local maxima, 1 global minimum and (at least) 2 local minima:
ECON 2050  Optimization I
5 / 25
```

## PDF page 6

```text
First-order necessary conditions for interior local extrema
First, we generalize the one-variable calculus necessary condition f ′(x) = 0:
Denition
Let D ⊆Rn, and f : D →R is a dierentiable function. Then x ∈intD is a critical point of f
if
∇f (x) = 0,
that is, if
∂f (x)
∂x1
= 0, ∂f (x)
∂x2
= 0, . . . , ∂f (x)
∂xn
= 0.
Theorem (First-order necessary condition)
Let D ⊆Rn, and f : D →R is a dierentiable function. If x ∈int D is a local extremum of f ,
then x is a critical point of f .
ECON 2050  Optimization I
6 / 25
```

## PDF page 7

```text
Proof sketch (two variable case):
Suppose f : R2 →R achieves a local maximum at point (x∗
1, x∗
2). Then
∃r > 0, ∀(x1, x2) ∈Br(x∗
1, x∗
2) :
f (x1, x2) ≤f (x∗
1, x∗
2)
Thus, if we keep x2 = x∗
2 xed and dene g : R →R given by g(x1) ≡f (x1, x∗
2),
∀x1 ∈pr1(Br(x∗
1, x∗
2)) :
g(x1) = f (x1, x∗
2) ≤f (x∗
1, x∗
2) = g(x∗
1)
This implies that the one variable function g has a local maximum at x1 = x∗
1, which implies
that g ′(x∗
1) = 0 and therefore
∂f (x∗
1, x∗
2)
∂x1
= 0
Analogously, keeping x1 = x∗
1 xed, we obtain ∂f (x∗
1 ,x∗
2 )
∂x2
= 0.
Changing ≤for ≥demonstrates the same result for a local minimum.
ECON 2050  Optimization I
7 / 25
```

## PDF page 8

```text
Example: Consider f : R2 →R, (x1, x2) ↦→x2
1 + x2
2.
To determine f 's critical points we calculate the partial derivatives and equate them to zero:
∂f (x1, x2)
∂x1
= 2x1 = 0
∂f (x1, x2)
∂x2
= 2x2 = 0
Solving the system, we obtain the only critical point (0, 0).
Because R2 is open (as any x ∈R2 is an interior point), we know from the previous theorem
that every (x1, x2) ̸= (0, 0) is neither a local maximum nor a local minimum.
However, we do not know if (0, 0) is a local maximum or a local minimum or neither.
ECON 2050  Optimization I
8 / 25
```

## PDF page 9

```text
To sum up: If D ⊆Rn is open and f : D →R is dierentiable,
non-critical points are not local extrema (and therefore not global extrema).
But: Not every critical point is say a local maximum, or even a local extremum. E.g., (0, 0) is
a critical point of all of the following functions (verify!), and
a local minimum for f : R2 →R, (x1, x2) ↦→x2
1 + x2
2
a local maximum of f : R2 →R, (x1, x2) ↦→−(x2
1 + x2
2)
2
4
−1
1
2
−2
2
4
x1
x2
y
2
4
−1
1
2
−2
x1
x2
y
ECON 2050  Optimization I
9 / 25
```

## PDF page 10

```text
a saddle point (= a critical point that is not a local extremum) of
f : R2 →R, (x1, x2) ↦→x2
1 −x2
2
−1
1
2
−1
1
2
−1
1
x1
x2
y
ECON 2050  Optimization I
10 / 25
```

## PDF page 11

```text
Sucient conditions
Above, we discussed that a necessary condition for a point to be a local extremum is that it is a
critical point.
In general we don't even know whether a critical point is a local extremum, let alone global
The following theorem shows that being a critical point is sucient for a global maximum
[minimum] of concave [convex] functions.
Theorem (Sucient conditions for global extrema)
Let D ⊆Rn be convex, f : D →R be a dierentiable function. Then:
1 Suppose f is concave, then x∗is a (global) maximum of f if it is a critical point of f .
2 Suppose f is convex, then x∗is a (global) minimum of f if it is a critical point of f .
ECON 2050  Optimization I
11 / 25
```

## PDF page 12

```text
Theorem (Sucient conditions for global extrema)
Let D ⊆Rn be convex, f : D →R be a dierentiable function. Then:
1 Suppose f is concave, then x∗is a (global) maximum of f if it is a critical point of f .
2 Suppose f is convex, then x∗is a (global) minimum of f if it is a critical point of f .
Proof: We only prove part 1; part 2 can be proved analogously. Since f is concave,
f (y) −f (x) ≤∇f (x) · (y −x),
∀x, y ∈D
(by the theorem on lecture 7 slide 26). If x ∗is a critical point of f then ∇f (x∗) = 0, meaning
that for all x ∈D,
f (x) −f (x∗) ≤0 · (x −x∗) = 0,
which is equivalent to f (x) ≤f (x∗) for all x ∈D. Hence x∗is a global maximum of f .
ECON 2050  Optimization I
12 / 25
```

## PDF page 13

```text
Example: The partial derivatives of f : R2 →R, (x, y) ↦→f (x, y) = x2 + y2 are
∂f (x, y)
∂x
= 2x,
∂f (x, y)
∂y
= 2y
The unique critical point of f is (0, 0). Since we know that f is convex (see, for example,
Lecture 7 slide 30), (0, 0) must be a global minimum of f .
ECON 2050  Optimization I
13 / 25
```

## PDF page 14

```text
Exercise: Determine the extrema of f : R2 →R given by f (x, y) = −x2 + xy −y2. Classify
them into local or global (you can use the fact that f is concave).
We calculate the critical points:
∂f (x, y)
∂x
= −2x + y = 0
∂f (x, y)
∂y
= −2y + x = 0
The only critical point is (0, 0). Because R2 is open, this is the only candidate for local extrema.
Since f is a concave function, (0, 0) is a global maximum and therefore also a local maximum.
ECON 2050  Optimization I
14 / 25
```

## PDF page 15

```text
Example: Consider f : R2
++ →R given by f (x1, x2) = ln
(︁
x2
1 + x2
2
)︁
.
To determine f 's critical points we calculate the partial derivatives and equate them to zero:
∂f (x1, x2)
∂x1
=
2x1
x2
1 + x2
2
= 0
∂f (x1, x2)
∂x2
=
2x2
x2
1 + x2
2
= 0
We see that f has no critical points in R2
++ (note that (0, 0) /∈R2
++).
Then because R2
++ is open, f has neither local maxima nor local minima.
Since every global maximum [minimum] is a local maximum [minimum], f has neither
global maximum nor global minimum.
ECON 2050  Optimization I
15 / 25
```

## PDF page 16

```text
Existence of global extrema
We mentioned the following important result in Lecture 2:
Theorem (Extreme Value Theorem)
Let D ⊆Rn be compact and f : D →R be continuous. Then f has at least one global
maximum and at least one global minimum. That is, there exist x max, xmin ∈D such that
f (xmax) ≥f (x) ≥f (xmin)
∀x ∈D.
Proof idea:
The key step is that the range of f , f (D), is a compact subset of R provided that f is
continuous and D is compact; thus, f (D) is closed and bounded.
Boundedness means that max f (D) and min f (D) are bounded away from innity, and
closeness implies that max f (D) and min f (D) can be attained.
ECON 2050  Optimization I
16 / 25
```

## PDF page 17

```text
Why do the conditions of the theorem matter?
Example: Let C = R and f : C →R be given by f (x) = x.
Then f is continuous, but C is not compact (closed but not bounded). Since f (C) = R, f has
neither a (global) maximum nor a minimum.
Example: Let D = (0, 1) and f : D →R be given by f (x) = x.
Then f is continuous, but D is again non-compact (bounded but not closed). Since
f (D) = (0, 1), f has neither a (global) maximum nor a minimum. (Note that x = 0 and x = 1
are not in D.)
ECON 2050  Optimization I
17 / 25
```

## PDF page 18

```text
Properties of maximization/minimization problems
Proposition
Let f : D →R, where D ⊆Rn, and let −f denote the function whose value at x is −f (x).
Then
x is a (global) maximum [minimum] of f if and only if x is a (global) minimum
[maximum] of −f ;
y is a local maximum [minimum] of f if and only of y is a local minimum [maximum] of
−f .
The above result tells us that a generic minimization problem
min
x∈D g(x)
is equivalent to
max
x∈D −g(x);
in other words, every minimization problem may be represented as a maximization problem.
ECON 2050  Optimization I
18 / 25
```

## PDF page 19

```text
The following result is useful for calculating (global or local) extrema since it allows us to
simplify the optimization problem.
Proposition
If h : R →R is an increasing function, D ⊆Rn, g : D →R and x is a maximum [minimum] of
g, then x is also a maximum [minimum] of h ◦g. If h : R →R is strictly increasing, the
maxima [minima] of h ◦g and g coincide.
Proof idea: compositing with an increasing function preserves maximality [minimality].
Example: Instead of minimizing
f (x, y) = ex2+y2,
we can minimize g(x, y) = x2 + y2  since h(z) = ez is strictly increasing and f = h ◦g, the
minima of f and g coincide.
ECON 2050  Optimization I
19 / 25
```

## PDF page 20

```text
Example: Let E = [−1, 1] and g : E →R be given by
g(x) =
{︃0,
if x = −1 or x = 1;
x,
if −1 < x < 1.
Note that E is compact, but f is not continuous at −1 and 1. In this case, g(E) = (−1, 1),
and hence f has neither a (global) maximum nor a minimum.
−1
1
−1
1
x
g(x)
ECON 2050  Optimization I
20 / 25
```

## PDF page 21

```text
Exercise: Check whether the conditions of the extreme value theorem hold, and nd the
(global) extrema if they exist.
1 C = [−1, 1] and f : C →R be given by f (x) = x2.
▶Both conditions hold because C is closed and bounded, and hence compact, and f is continuous
▶By the extreme value theorem, a maximum and a minimum exist.
▶x = −1 and x = 1 are global maxima and x = 0 is a global minimum.
2 C = [−1, 1] and g : C →R be given by
g(x) =
{︄
x
if −1 ≤x ≤0,
1 −x2
if 0 < x ≤1.
▶C is compact but g is discontinuous at x = 0; the extreme value theorem doesn't apply.
▶There is no global maximum, but x = −1 is a global minimum.
ECON 2050  Optimization I
21 / 25
```

## PDF page 22

```text
Caveats:
The theorem does not say where these extrema are or how to nd them, it only says that
these points exist.
Importantly, the conditions of the theorem are not necessary: if one or more of the
conditions fails, maxima and minima may still exist.
Example: Let D = [−1, ∞), and let f : D →R be dened by
f (x) =
{︄
x
if −1 ≤x < 0,
1
if x ≥0.
We see that f is not continuous at x = 0 ∈D, and D is not compact (closed but not
bounded); but any x ≥0 is a global maximum of f , and x = −1 is a global minimum.
ECON 2050  Optimization I
22 / 25
```

## PDF page 23

```text
A (not-always-useful) cookbook procedure for nding (global) extrema
Let S be a compact subset of Rn, and let f : S →R be continuous. Then the extrema of f can
be found as follows:
1 Find all critical points in intS.
2 Among the points in S\intS (i.e., the boundary points), nd those at which the value of f
is largest.
3 Among all the points you have found in the previous two steps, the ones at which the
value of f are the largest [smallest] are the (global) maxima [minima].
This approach is not always useful, because evaluating all boundary points can be dicult.
In the next three lectures, we will discuss a simpler and more systematic approach.
However, in certain cases, this approach can be handy.
ECON 2050  Optimization I
23 / 25
```

## PDF page 24

```text
Example: Consider the minimization problem min(x,y)∈S f (x, y), where f : R2 →R is given by
f (x, y) = x2 + y2, and
S =
{︁
(x, y) ∈R2 : 1 ≤x + y ≤3, x ≥0, y ≥0
}︁
.
We know from slide 13 that no interior point of S is a solution, because the unique critical
point (0, 0) is not in S.
However, by the extreme value theorem, the minimization problem has a solution.
So: Which of the boundary points are solutions?
ECON 2050  Optimization I
24 / 25
```

## PDF page 25

```text
Below, we depict S =
{︁
(x, y) ∈R2 : 1 ≤x + y ≤3, x ≥0, y ≥0
}︁
and some level curves of f .
The graph shows that the unique solution of the minimization problem is ( 1
2, 1
2).
In fact, we can say more: (3, 0) and (0, 3) maximize f on S.
ECON 2050  Optimization I
25 / 25
```
