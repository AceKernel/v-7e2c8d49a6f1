# Tutorial 8 solutions: automatic text transcript

Original: [Tutorial 8 solutions PDF](tutorial-08-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050
S2 2026
Tutorial 8 Solution
Problem 1
In lecture 7, we learned about a result that if f = h ◦g, where h is increasing and
convex, and g is convex, then f is also convex. We have also seen examples where the
“outer function” h is convex but not increasing and therefore the composition fails to be
convex.
However, if the “inner function” g is not just convex, but affine, then even if the “outer
function” h is convex but not increasing, the composition h ◦g is still convex.
(a) Prove the fact stated in the second paragraph; that is, if g : S →R is affine and h : R →
R is convex, where S ⊆Rn, then the composition f ≡h ◦g is convex. (Similarly, if g is
affine and h is concave, then the composition h ◦g is concave.)
(b) Use the fact in part (a) to show that
• f1(x, y) = (y −x)2 is convex; and
• f2(x, y) = −x2 −5y2 −4xy is concave.
(c) Find the global minima of f1(x, y).
(d) Find the global maxima of f2(x, y).
Solution:
(a) We need to show that f = h◦g is convex; that is, for any x1, x2 ∈S and every λ ∈[0, 1],
f (λx1 + (1 −λ)x2) ≤λf (x1) + (1 −λ)f (x2) ,
or equivalently,
h(g (λx1 + (1 −λ)x2)) ≤λh(g (x1)) + (1 −λ)h(g((x2)).
(1)
Since g is affine, it is both convex and concave, meaning that for any x1, x2 ∈S and
every λ ∈[0, 1],
g (λx1 + (1 −λ)x2) = λg (x1) + (1 −λ)g (x2) ;
thus,
h(g (λx1 + (1 −λ)x2)) = h(λg (x1) + (1 −λ)g (x2)).
(2)
Since h is convex, for any z1, z2 ∈R and every λ ∈[0, 1],
h (λz1 + (1 −λ)z2) ≤λh (z1) + (1 −λ)h (z2) .
Taking z1 ≡g(x1) and z2 ≡g(x2), inequality (2) implies
h(g (λx1 + (1 −λ)x2)) = h(λg (x1)+(1−λ)g (x2)) ≤λh(g (x1))+(1−λ)h(g((x2)),
which yields the desired inequality (1). Thus, f = h ◦g is a convex function.
1
```

## PDF page 2

```text
ECON 2050
S2 2026
(b) f1(x, y) = (y −x)2 is convex because f1 = h1 ◦g1, where h1(z) = z2 is convex and
g1(x, y) = x −y is linear (and therefore affine).
For f2, note that
f2(x, y) = −x2 −5y2 −4xy = −(x2 + 4xy + 4y2) −y2 = −(x + 2y)2 −y2.
By the fact we proved in part (a), we know that g2(x, y) := −(x + 2y)2 is concave
because g2 = u ◦v, where u(z) = −z2 is concave and v(x, y) = x + 2y is linear (and
therefore affine). Also, it is not difficult to see (for example, Tutorial 7 problem 2) that
h2(x, y) = −y2 is concave. Then since f2(x, y) = g2(x, y)+h2(x, y), f2(x, y) is concave.
(c) From
∂f1(x, y)
∂x
= −2(y −x) = 0
⇐⇒
y = x
∂f1(x, y)
∂y
= 2(y −x) = 0
⇐⇒
y = x
we see that (x, y) ∈R2 is a critical point of f1 if and only if y = x. By part (b), f is
convex, and therefore all the critical points, namely the points on the line determined
by y = x, are global minima.
(d) From
∂f2(x, y)
∂x
= −2x −4y = 0
∂f2(x, y)
∂y
= −10y −4x = 0
we deduce that the only critical point of f is (x∗, y∗) = (0, 0). Since we determined in
part (b) that f2 is concave, (x∗, y∗) = (0, 0) is the unique global maximum.
Problem 2
Calculate the critical points of the function f : C →R given by
f(x, y) = ln(8y −x2 + 4x),
and find out all its local or global extrema (i.e., maxima or minima).
Solution: Since h(z) = ln z is a strictly increasing function, by a theorem in the lecture, the
local and global maxima [minima] of g : D →R given by g(x, y) = 8y −x2 + 4x coincide
with the local and global maxima [minima] of f = h ◦g, respectively. From
∂g(x, y)
∂x
= −2x + 4 = 0
⇐⇒
x = 2
∂g(x, y)
∂y
= 8 = 0
⇐⇒
impossible
we conclude that no critical points exist.
Since C is an open set (see the graphical illustration below), every (x, y) ∈C that is not
a critical point cannot be a local extremum, and hence cannot be a global extremum either.
Thus, no local or global extremum exists.
2
```

## PDF page 3

```text
ECON 2050
S2 2026
x
y
Shaded region: C
(equivalent to {(x, y) ∈R2 : y > (x−2)2
8
−1
2})
Black dashed curve: boundary
(8y −x2 + 4x = 0, not contained in C)
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
Problem 4 (Extra Practice Problem)
An artisan uses xh units of labor and xm units of a unique material to produce a product.
Her profits if employing (xh, xm) ≥0 units of the mentioned factors are
π(xh, xm) = 20xh + 26xm + 4xhxm −4x2
h −3x2
m
Find the values of xh and xm that maximize the artisan’s profits.
Solution: To find the global maxima of π, first show that the objective function π is concave.
To that end, observe that if the term 4xhxm is absent, then π(xh, xm) can be written as the
sum of two functions, one is a function of xh only, and the other is a function of xm only,
and both functions are concave. If this is the case, π must also be concave by the result in
Tutorial 7 Problem 2. Therefore, we aim to “eliminate” the term 4xhxm by completing the
square.
Note that −4x2
h + 4xhxm −x2
m = −(2xh −xm)2, and therefore
π(xh, xm) = 20xh + 26xm −2x2
m −(2xh −xm)2.
Let π1(xh, xm) ≡20xh + 26xm −2x2
m; by the result in Tutorial 7 Problem 2, it is a concave
function. Also let π2(xh, xm) ≡−(2xh −xm)2; by the result in Problem 1, π2 is also a
concave function. Then since π = π1 + π2, and the sum of concave functions is a concave
function, π is also concave.
From
∂π(xh, xm)
∂xh
= 20 + 4xm −8xh = 0
⇐⇒
5 + xm = 2xh
∂π(xh, xm)
∂xm
= 26 + 4xh −6xm = 0
⇐⇒
3xm −13 = 2xh
4
```

## PDF page 5

```text
ECON 2050
S2 2026
we see that the unique critical point of π is (x∗
h, x∗
m) = (7, 9). Since π is concave, the unique
critical point (x∗
h, x∗
m) = (7, 9) must be a global maximum.
Summarizing, choosing xh = 7 and xm = 9 maximizes the artisan’s profits.
5
```
