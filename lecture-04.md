# Lecture 4: automatic text transcript

Original: [Lecture 4 PDF](lecture-04.pdf). Topic: Multivariable chain rule, Hessian and implicit functions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050 – Mathematical Economics
Basic Real Analysis IV
ECON 2050 – Basic Real Analysis IV
1 / 25
```

## PDF page 2

```text
The simplest chain rule: A review
In the previous lecture, we discussed the following result, usually referred to as the chain rule:
Theorem
Let D ⊆R be open, and let f : D →R be differentiable at x ∈D. Let g : E →R, where
f (D) ⊆E, be differentiable at f (x), then the composition g ◦f is differentiable at x, and
[(g ◦f )(x)]′ = g′(f (x))f ′(x).
This rule works nicely when we work with two functions of one variable.
ECON 2050 – Basic Real Analysis IV
2 / 25
```

## PDF page 3

```text
However, sometimes we are interested in situations where the “outer function” is a function of
several variables, and all variables are affected by the same parameter.
Example: Suppose the production function of a company is F(K, L), where K and L denote
capital and labor, respectively. It is natural to assume that both capital and labor accumulate
over time.
In this example, denoting time by t, we see that both K and L are functions of t.
ECON 2050 – Basic Real Analysis IV
3 / 25
```

## PDF page 4

```text
A more general chain rule
Theorem
Suppose that f : Rk →R is differentiable, and for each j = 1, 2, . . . , k, gj : Rm →R is
differentiable. Then the function F : R →R given by
F(x) ≡f (g1(x), . . . , gk(x))
is differentiable, and
F ′(x) = f1(g1(x), . . . , gk(x))g′
1(x) + . . . + fk(g1(x), . . . , gk(x))g′
k(x),
where fj is the partial derivative of f with respect to its j-th coordinate.
ECON 2050 – Basic Real Analysis IV
4 / 25
```

## PDF page 5

```text
Example (cont’d): Suppose further that at a given moment in time,
the marginal product of labor is 2.5 and the marginal product of capital is 3,
the amount of capital is increasing by 2 each unit of time and the rate of change of labor
is 0.5.
What is the rate of change of output?
The first bullet point indicates that
∂F(K, L)
∂K
= 3,
and
∂F(K, L)
∂L
= 2.5.
By the second bullet point, we know that K ′(t) = 2 and L′(t) = 0.5. Then by the
(generalized) chain rule,
dF
dt = ∂F(K, L)
∂K
K ′(t) + ∂F(K, L)
∂L
L′(t) = 2.5 · 2 + 3 · 0.5 = 6.5.
ECON 2050 – Basic Real Analysis IV
5 / 25
```

## PDF page 6

```text
Exercise: Consider the production function Q = 2K 2L. Suppose that the inputs K and L vary
with the interest rate r, via the expressions
K(r) =
1
ln(r + 1),
and
L(r) = 100 + 25r.
What is the rate of change of output Q?
We apply the chain rule:
dQ
dr = ∂Q
∂K · K ′(r) + ∂Q
∂L · L′(r)
= 4K(r)L(r) ·
(︃
−
1
(r + 1)[ln(r + 1)]2
)︃
+ 2K 2(r) · 25
= −
400 + 100r
(r + 1)[ln(r + 1)]3 +
50
[ln(r + 1)]2 .
ECON 2050 – Basic Real Analysis IV
6 / 25
```

## PDF page 7

```text
The theorem above also suggests a natural generalization of the chain rule to the case where
the “inside functions” are also functions of several variables.
Theorem
Suppose that f : Rk →R is differentiable, and for each j = 1, 2, . . . , k, gj : R →R is
differentiable. Then the function G : Rm →R given by
F(x) ≡f (g1(x), . . . , gk(x))
is differentiable, and for each i = 1, . . . , m,
∂F(x)
∂xi
= f1(g1(x), . . . , gk(x))∂g1(x)
∂xi
+ . . . + fk(g1(x), . . . , gk(x))∂gk(x)
∂xi
,
where xi is the i-th coordinate of x, fj is the partial derivative of f with respect to its j-th
coordinate.
ECON 2050 – Basic Real Analysis IV
7 / 25
```

## PDF page 8

```text
Second-order derivatives
Intuitively, higher-order derivatives are the result of differentiating a function repeatedly.
Consider a differentiable function f : D →R, where D is an open subset of R. Consider the
“derivative function” x ↦→f ′(x); we denote it by f ′.
The derivative of f ′ at x is called the second-order derivative of f at x, and is written f ′′(x).
We may go on to define even higher order derivatives (third, fourth, etc.), but we don’t need
those in this course.
Example: Consider the function f (x) = x2. Its (first-order) derivative is f ′(x) = 2x, and its
second-order derivative is f ′′(x) = 2.
ECON 2050 – Basic Real Analysis IV
8 / 25
```

## PDF page 9

```text
Second-order partial derivatives
Let D ⊆Rk be open. If f : D →R is partially differentiable, then, if they exist, the partial
derivatives of the functions
∂f
∂xi
: D →R, x ↦→∂f (x)
∂xi
,
∀i = 1, . . . , k,
are called the second-order partial derivatives of f . For j = 1, . . . , k, we write
∂2f (x0)
∂xi∂xj
or
fxixj(x0)
for the partial derivative
∂
(︂
∂f
∂xi
)︂
(x0)
∂xj
of ∂f
∂xi at x0 with respect to xj.
ECON 2050 – Basic Real Analysis IV
9 / 25
```

## PDF page 10

```text
A twice partially differentiable function f : R2 →R, (x, y) ↦→f (x, y) has 4 second-order partial
derivatives. We write ∂x2 for ∂x∂x etc.:
1
∂2f
∂x2 = fxx = second-order partial derivative of f with respect to x and x
2
∂2f
∂x∂y = fxy = second-order partial derivative of f with respect to x and y
3
∂2f
∂y∂x = fyx = second-order partial derivative of f with respect to y and x
4
∂2f
∂y2 = fyy = second-order partial derivative of f with respect to y and y
Cases 2 and 3 are called mixed or cross-partial derivatives.
ECON 2050 – Basic Real Analysis IV
10 / 25
```

## PDF page 11

```text
Example: To obtain the second-order partial derivatives of
f : R2 →R, (x, y) ↦→exy,
we first calculate the first-order partial derivatives
∂f (x, y)
∂x
= yexy;
∂f (x, y)
∂y
= xexy
and then differentiate these with respect to x and with respect to y:
∂2f (x, y)
∂x2
=
y2exy;
∂2f (x, y)
∂x∂y
= exy + yxexy = exy(1 + xy)
∂2f (x, y)
∂y2
=
x2exy;
∂2f (x, y)
∂y∂x
= exy + yxexy = exy(1 + xy)
Observe that here, the cross partial derivatives are equal.
ECON 2050 – Basic Real Analysis IV
11 / 25
```

## PDF page 12

```text
This is often the case in economic applications. The following theorem provides sufficient
condition for the cross-partial derivatives to be equal.
Theorem (Young’s Theorem)
If D ⊆Rk is open and f : D →R twice continuously partially differentiable, then
∂2f
∂xi∂xj
=
∂2f
∂xj∂xi
,
∀xi, xj
If Young’s theorem holds, the order of differentiation does not matter. (In the previous
example, Young’s theorem applied.)
ECON 2050 – Basic Real Analysis IV
12 / 25
```

## PDF page 13

```text
Hessian matrix
Let D ⊆Rk be open, and f : D →R be twice partially differentiable.
The Hessian matrix Hf (x0) of f at x0 consists of all its second-order partial derivatives of f
at x0:
Hf (x0) =
⎛
⎜
⎜
⎝
fx1x1(x0)
fx1x2(x0)
...
fx1xk(x0)
fx2x1(x0)
fx2x2(x0)
...
fx2xk(x0)
...
...
...
...
fxkx1(x0)
fxkx2(x0)
...
fxkxk(x0)
⎞
⎟
⎟
⎠
If Young’s theorem holds (which we will assume from now on) this matrix is symmetric (that
is, for all i and all j, the entry in the i-th row and j-th column equals the entry in the j-th row
and the i-th column).
ECON 2050 – Basic Real Analysis IV
13 / 25
```

## PDF page 14

```text
Example (ct’ed): The Hessian matrix of
f : R2 →R, (x, y) ↦→exy,
at (x, y) is
Hf (x, y) =
(︃fxx(x, y)
fxy(x, y)
fyx(x, y)
fyy(x, y)
)︃
=
(︃
y2exy
exy(1 + xy)
exy(1 + xy)
x2exy
)︃
ECON 2050 – Basic Real Analysis IV
14 / 25
```

## PDF page 15

```text
Implicit functions
Example: The level curves of the function f : R2 →R, (x, y) ↦→x2 + y2 have the form
x2 + y2 = C.
(1)
Each of f ’s level curves defines a function of one variable, as we can see by rearranging (1) as:
y =
√︁
C −x2.
(2)
The difference between expressions (1) and (2) is that
in (1) the variable y appears in the “implicit” form (not separated) and
in (2) it appears in the “explicit” form (separated).
ECON 2050 – Basic Real Analysis IV
15 / 25
```

## PDF page 16

```text
However, we cannot always solve for y. For example, consider
y5 −5xy + 4x4 = 0,
(3)
an equation describing a level curve of f : R2 →R, (x, y) ↦→y5 −5xy + 4x4.
Note that (x0, y0) = (1, 1) lies on this level curve, as it solves (3).
Questions:
Can we still describe the level curve given by (3) as a function of one variable, at least
“around” the point (x0, y0) = (1, 1)?
If so, is this function differentiable? What is its slope?
ECON 2050 – Basic Real Analysis IV
16 / 25
```

## PDF page 17

```text
Why do we care?
Suppose a firm’s profit function, which is a function of both the price of the product p and the
input price c, is Π(p, c).
We know from ECON1050 or ECON2010 that if we wish to choose a price to maximize the
profits, a necessary condition is the so-called “first-order condition”
∂Π(p, c)
∂p
= 0.
If we wish to understand how does the optimal price p∗, which is a solution to the first-order
condition, varies in c:
for sufficiently simple profit functions we can explicitly write p∗as a function of c: if
Π(p, c) = 2pc −p2/2, the first-order condition is 2c −p∗= 0, and therefore p∗= 2c
however, for slightly more complicated profit functions, this may not be possible
we may, nonetheless, be interested in understanding how the optimal price should change
when there is a small change in the input price
ECON 2050 – Basic Real Analysis IV
17 / 25
```

## PDF page 18

```text
Observation: In the previous example (level curves of the function f (x, y) = x2 + y2), the
expression y =
√
C −x2 may not define a function around certain points on the level curve.
y
x
a
b
x2 + y2 = C
Around point a, y can be seen as a function of x: y = g(x) :=
√
C −x2; however, y doesn’t
define a function around point b.
ECON 2050 – Basic Real Analysis IV
18 / 25
```

## PDF page 19

```text
Theorem (Implicit function theorem)
Suppose G(x, y) is a continuously differentiable real-valued function defined on an open set
containing (x0, y0). If G(x0, y0) = C, and
∂G(x0, y0)
∂y
̸= 0,
then there exists a δ > 0 and a continuously differentiable function g : Bδ(x0) →R such that
G(x, g(x)) = C for all x ∈Bδ(x0),
g(x0) = y0, and
g′(x0) = −
∂G(x0, y0)
∂x
∂G(x0, y0)
∂y
.
Intuitively, if the assumptions of the theorem hold, even though y cannot be isolated in the
original equation G(x, y) = C, the derivative of y with respect to x around the point (x0, y0)
can be isolated in terms of the partial derivatives of G.
ECON 2050 – Basic Real Analysis IV
19 / 25
```

## PDF page 20

```text
To get some intuition for the condition ∂G(x0,y0)
∂y
̸= 0, consider the equation (level curve)
x2 + y2 = 1 and
G(x, y) = x2 + y2 = 0
For this G,
∂G(x, y)
∂y
= 2y
and ∂G(x,y)
∂y
= 0 if and only if y = 0.
If y0 = 0, then x0 = 1, and there is no δ > 0 such that we can describe the level curve by a
function g : Bδ(x0) →R: take any ε ∈(0, δ), along the curve,
if we increase x a bit to x = 1 + ε, then there is no corresponding y so that (1 + ε, y)
solves the equation;
if we decrease x a little to x = 1 −ε, then there are two equally good candidates for y
near y = 0, namely y1 =
√
2ε −ε2 and y2 = −
√
2ε −ε2.
ECON 2050 – Basic Real Analysis IV
20 / 25
```

## PDF page 21

```text
To understand the formula for g′(x), note that by definition, if we move along a level curve of
G, then the value of G does not change.
Recall that we can approximate the change in G from a change (dx, dy) in its variables by
DG(x0, g(x0)) · (dx, dy) = ∂G(x0, g(x0))
∂x
dx + ∂G(x0, g(x0))
∂y
dy
If we (approximately) move along a level curve, then
∂G(x0, g(x0))
∂x
dx + ∂G(x0, g(x0))
∂y
dy = 0
and rearranging yields
dy
dx = g′(x) = −
∂G(x0,g(x0))
∂x
∂G(x0,g(x0))
∂y
ECON 2050 – Basic Real Analysis IV
21 / 25
```

## PDF page 22

```text
Example: Consider the equation x2 −3xy + y3 = 7 around the point (x0, y0) = (4, 3).
Consider the level curve of level 7 of the function G(x, y) = x2 −3xy + y3. One can show that
∂G(x, y)
∂x
= 2x −3y,
and
∂G(x, y)
∂y
= −3x + 3y2;
because both partial derivatives are continuous, G must be continuously differentiable.
Moreover, G(4, 3) = 7 and ∂G(4,3)
∂y
= 15 ̸= 0.
Then by the implicit function theorem, one can write y as a continuously differentiable
function of x, denoted by g(x), around (4, 3), and
g′(4) = −
∂G(4,3)
∂x
∂G(4,3)
∂y
= 1
15.
We can also write down the tangent line h to the level curve at the point (x0, y0) = (4, 3):
h(x) = y0 + g′(x0)(x −x0) = 3 + 1
15(x −4) = 1
15x + 1
3.
ECON 2050 – Basic Real Analysis IV
22 / 25
```

## PDF page 23

```text
Exercise: Does the equation xy ln(xy) = 0 define a function y = g(x) around (1, 1)? What is
its derivative at x0 = 1?
Consider the level curve of level 0 of f (x, y) = xy ln(xy).
The conditions of the implicit function theorem are fulfilled with respect to f :
∂f (x,y)
∂x
= y ln(xy) + y and ∂f (x,y)
∂y
= x ln(xy) + x, f is continuously differentiable because
both partial derivatives are continuous;
f (1, 1) = 0; and
∂f (1,1)
∂y
= 1 ̸= 0.
Hence y can be written as a function of x, denoted by g(x), and we can calculate its
derivative at x0 = 1 as
g′(1) = −
∂f (1,1)
∂x
∂f (1,1)
∂y
= −0 + 1
0 + 1 = −1
ECON 2050 – Basic Real Analysis IV
23 / 25
```

## PDF page 24

```text
Implicit function theorem: General case
Theorem
Suppose x0 ∈Rm, y0 ∈R, and G(x, y) is a continuously differentiable real-valued function
defined on an open set containing (x0, y0). If
G(x0, y0) = C
and
∂G(x0, y0)
∂y
̸= 0,
then there exists a δ > 0 and a continuously differentiable function g : Bδ(x0) →R such that
G(x, g(x)) = C for all x ∈Bδ(x0),
g(x0) = y0, and
∂g(x0)
∂xi
= −
∂G(x0, y0)
∂xi
∂G(x0, y0)
∂y
for all i = 1, . . . , m.
ECON 2050 – Basic Real Analysis IV
24 / 25
```

## PDF page 25

```text
Example: Consider the equation x3 + y3 + z3 −3z = 0.
By the implicit function theorem this equation defines a function z of x and y in a
neighborhood of every point (x0, y0, z0) for which A) the equation holds and B)
∂f (x0,y0,z0)
∂z
̸= 0, where f (x, y, z) = x3 + y3 + z3 −3z.
We can calculate the partial derivatives of z by using the partial derivatives of the function f .
∂z(x0, y0)
∂x
=
−
∂f (x0,y0,z0)
∂x
∂f (x0,y0,z0)
∂z
= −
3x2
0
3z2
0 −3
∂z(x0, y0)
∂y
=
−
∂f (x0,y0,z0)
∂y
∂f (x0,y0,z0)
∂z
= −
3y2
0
3z2
0 −3
ECON 2050 – Basic Real Analysis IV
25 / 25
```
