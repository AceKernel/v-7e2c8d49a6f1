# Lecture 3: automatic text transcript

Original: [Lecture 3 PDF](lecture-03.pdf). Topic: Differentiability, partials, gradient and approximation.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050 – Mathematical Economics
Basic Real Analysis III
ECON 2050 – Basic Real Analysis III
1 / 31
```

## PDF page 2

```text
Differentiability: Functions of one variable
Recall the definition of differentiability for functions of one variable:
Definition
Let D ⊆R be open. The function f : D →R is differentiable at x ∈D if there exists
f ′(x) ∈R such that
f ′(x) = lim
n→∞
f (x + hn) −f (x)
hn
for all sequences (hn) with hn →0 and hn ̸= 0 for all n. In this case, f ′(x) is called the
derivative of f at x.
Equivalently, f : D →R is differentiable at x0 if and only if there exists a ∈R such that
lim
n→∞
f (x0 + hn) −f (x0) −ahn
hn
= 0
for all sequences (hn) with hn →0 and hn ̸= 0 for all n. In this case, a = f ′(x0).
ECON 2050 – Basic Real Analysis III
2 / 31
```

## PDF page 3

```text
x
x + hn
f (x)
f (x + hn)
secant line
x
f (x)
x
f (x)
tangent line
slope = f ′(x)
ECON 2050 – Basic Real Analysis III
3 / 31
```

## PDF page 4

```text
Below are a list of results that are treated as well understood from previous courses in calculus
and high school
f (x)
f ′(x)
k
0
kxn
knxn−1
ln x
1/x
ex
ex
cos x
−sin x
sin x
cos x
where k ∈R is a constant.
ECON 2050 – Basic Real Analysis III
4 / 31
```

## PDF page 5

```text
The following results may also be familiar. These will be very useful throughout the course.
Theorem (Rules of differentiation)
Let D ⊆R be open, and let f : D →R and g : D →R be differentiable at x ∈D. Then
f + g, fg, and f /g are differentiable at x, and
(1) [f (x) + g(x)]′ = f ′(x) + g′(x);
(2) [f (x)g(x)]′ = f ′(x)g(x) + f (x)g′(x); and
(3) if g(x) ̸= 0,
[︃f (x)
g(x)
]︃′
= g(x)f ′(x) −g′(x)f (x)
[g(x)]2
.
ECON 2050 – Basic Real Analysis III
5 / 31
```

## PDF page 6

```text
These exercises are provided to ”refresh” your calculus.
Exercises:
Calculate the derivative of h(x) = x ln x.
h′(x) = ln x + x
(︃1
x
)︃
= ln x + 1.
Calculate the derivative of ˆh(x) = ex/x.
ˆh′(x) = exx −ex
x2
= ex x −1
x2 .
ECON 2050 – Basic Real Analysis III
6 / 31
```

## PDF page 7

```text
Theorem (Chain rule)
Let D ⊆R be open, and let f : D →R be differentiable at x ∈D. Let g : E →R, where
f (D) ⊆E, be differentiable at f (x), then the composition g ◦f is differentiable at x, and
[(g ◦f )(x)]′ = g′(f (x))f ′(x).
The chain rule is often summarized as “the derivative of the outside times the derivative of the
inside,” but one must remember that the derivative of the outside function is evaluated at the
inside function’s value at x.
ECON 2050 – Basic Real Analysis III
7 / 31
```

## PDF page 8

```text
Exercises:
Calculate the derivative of ˜h(x) = ln(x2 + 4).
We first observe that ˜h(x) = (˜g ◦˜f )(x), where ˜g(y) ≡ln y, and ˜f (x) ≡x2 + 4.
By the chain rule,
˜h′(x) = ˜g′(˜f (x))˜f ′(x) = [ln(˜f (x))]′ ˜f ′(x) =
1
˜f (x)
˜f ′(x) =
2x
x2 + 4.
Calculate the derivative of ¯h(x) = e1/x.
We first observe that ¯h(x) = (¯g ◦¯f )(x), where ¯g(y) ≡ey, and ¯f (x) ≡1/x.
By the chain rule,
¯h′(x) = ¯g′(¯f (x))¯f ′(x) =
[︂
e
˜f (x)]︂′ ˜f ′(x) = e
˜f (x) ˜f ′(x) = −e
1
x
x2 .
ECON 2050 – Basic Real Analysis III
8 / 31
```

## PDF page 9

```text
Differentiability: Functions of several variables
In the remainder of today’s lecture, we generalize the idea of differentiation to functions of
several variables.
ECON 2050 – Basic Real Analysis III
9 / 31
```

## PDF page 10

```text
(Total) differentiability
Definition
Let D ⊆Rk be open. The function f : D →R is (totally) differentiable at x ∈D if there
exists a ∈Rk such that
lim
n→∞
|f (x + hn) −f (x) −a · hn|
∥hn∥
= 0
for all sequences (hn) with hn →0 and hn ̸= 0 for all n. In this case, we call Df (x) ≡a the
derivative of f at x.
If f is differentiable at x for all x ∈D, then we say that f is differentiable. If in addition, the
“derivative function” x ↦→Df (x) is continuous, then we call f continuously differentiable.
ECON 2050 – Basic Real Analysis III
10 / 31
```

## PDF page 11

```text
The definition can be a bit abstract, but the geometric intuition should be straightforward,
which is a natural generalization of the differentiability concept for functions of one variable.
If k = 1,
▶Df (x0) ∈R is a number and
▶g is a tangent line of f at x0.
If k = 2,
▶Df (x0) ∈R2 is a
pair
of numbers and
▶g is a tangent
plane
of f at x0.
If k = n,
▶Df (x0) ∈Rn is a vector of numbers and
▶g is a tangent hyperplane of f at x0.
Once we know the tangent hyperplane g to f at x0, we can use it as an approximation of
f in the neighborhood of x0.
ECON 2050 – Basic Real Analysis III
11 / 31
```

## PDF page 12

```text
Example:
In blue, the graph of f : R2 →R, (x1, x2) ↦→1
3(x2
1 + x2
2).
In red, the graph of g : R2 →R, (x1, x2) ↦→f (1.5, 1.5) + (1, 1) · (x1 −1.5, x2 −1.5).
g is tangent to f at x0 = (1.5, 1.5), and we claim that Df (1.5, 1.5) =
(1,1)
.
ECON 2050 – Basic Real Analysis III
12 / 31
```

## PDF page 13

```text
The (total) derivative of f allows us to approximate f “in any direction.”
A second type of derivative of f just asks how y = f (x) changes if we move in a
particular direction from x0.
Such an idea is usually captured by the concept of “directional derivative”
For now, we consider a special case, where we only move in a single dimension/element,
say, xi
ECON 2050 – Basic Real Analysis III
13 / 31
```

## PDF page 14

```text
Partial derivatives
Definition
Let f : D →R, with D ⊆Rk open. If for all sequences (hn) with hn →0 and hn ̸= 0 for all n,
lim
n→∞
f (x1, ..., xi + hn, ..., xk) −f (x1, ..., xi, ..., xk)
hn
exists and equals to the same finite real number, then we denote this limit by ∂f (x)
∂xi , and say
that f is partially differentiable at x with respect to xi. In this case, ∂f (x)
∂xi
is called the
partial derivative of f at x with respect to xi.
If f is partially differentiable at x with respect to all xi, then we call it partially differentiable
at x. If If f is partially differentiable at all x ∈D, we call it partially differentiable. If, in
addition, all partial derivatives of f are continuous, then we call f continuously partially
differentiable.
ECON 2050 – Basic Real Analysis III
14 / 31
```

## PDF page 15

```text
For example, if they exist, the partial derivatives of a function f : R2 →R are
∂f (x, y)
∂x
= lim
n→∞
f (x + hn, y) −f (x, y)
hn
∂f (x, y)
∂y
= lim
n→∞
f (x, y + hn) −f (x, y)
hn
Like calculating derivatives of functions of one variables, we can sometimes calculate
partial derivatives directly from the definition, that is, by directly determining
corresponding the limit
However, it is much easier to apply the methods for differentiation of a single variable to
this setting. That is, we differentiate with respect to the variable of interest whilst
”holding all others constant”.
Sometimes we wish to to calculate the partial derivatives at a point of interest; to that
end, we first calculate the partial derivative functions and evaluate it at the point.
ECON 2050 – Basic Real Analysis III
15 / 31
```

## PDF page 16

```text
Example: The partial derivatives of f : R2 →R, (x1, x2) ↦→1
3(x2
1 + x2
2) are
∂f (x1, x2)
∂x1
= 2
3x1
∂f (x1, x2)
∂x2
= 2
3x2
The partial derivatives at (x1, x2) = (1.5, 1.5) are:
∂f (1.5, 1.5)
∂x1
= ∂f (1.5, 1.5)
∂x2
= 2
3 · 1.5 = 1
Similar to a derivative of a function of one variable, the partial derivative ∂f (x0)
∂xi
represents
the instantaneous rate of change f at x0 with respect xi.
∂f (1.5,1.5)
∂x1
= 1 signifies that the value of f at point (1.5, 1.5) increases by one unit for a
unit increase in x1 while holding x2 fixed.
ECON 2050 – Basic Real Analysis III
16 / 31
```

## PDF page 17

```text
Exercises:
Calculate the partial derivatives of g(x, y) = x2 + xy + y + 1.
∂g(x, y)
∂x
= 2x + y,
∂g(x, y)
∂y
= x + 1.
Calculate the partial derivatives of h(x, y) = exy + y ln x + 3.
∂h(x, y)
∂x
= yexy + y
x ,
∂h(x, y)
∂y
= xexy + ln x.
ECON 2050 – Basic Real Analysis III
17 / 31
```

## PDF page 18

```text
Some partial derivatives in Economics
Sometimes, partial derivatives are so important that economists give them special names:
Consider a production function F : R2
++ →R, (K, L) ↦→Q(K, L).
▶
∂F
∂K is called the
marginal product of capital
.
▶
∂F
∂L is called the
marginal product of labor
.
Consider a utility function u : Rk
++ →R, x ↦→u(x).
▶
∂u
∂xi is called the
marginal utility of good i
.
ECON 2050 – Basic Real Analysis III
18 / 31
```

## PDF page 19

```text
Geometric interpretation of partial derivatives
We can interpret the graph of x ↦→f (x, b) (green) as a curve at the intersection of the graph
of f : R2 →R, (x, y) ↦→f (x, y) and the plane {(x, y, z) ∈R3 : y = b} (red), and ∂f (a,b)
∂x
as
the slope of the tangent line (yellow) to this curve at (a, b, f (a, b)).
ECON 2050 – Basic Real Analysis III
19 / 31
```

## PDF page 20

```text
We can interpret the graph of y ↦→f (a, y) (green) as a curve at the intersection of the graph
of f : R2 →R, (x, y) ↦→f (x, y) and the plane {(x, y, z) ∈R3 : x = a} (red), and ∂f (a,b)
∂y
as
the slope of the tangent line (yellow) to this curve at (a, b, f (a, b)).
ECON 2050 – Basic Real Analysis III
20 / 31
```

## PDF page 21

```text
Relation between partial and total derivatives
One way to derive [Df (x0)]1 and [Df (x0)]2 analytically is by exploiting the fact that g is affine
and we can thus “decompose” dy = g(x0 + dx) −g(x0):
dy = dy1 + dy2 = [Df (1.5, 1.5)]1dx1 + [Df (1.5, 1.5)]2dx2 = 1 · dx1 + 1 · dx2
ECON 2050 – Basic Real Analysis III
21 / 31
```

## PDF page 22

```text
Let D ⊆Rk be open. We define the gradient ∇f (x0) of f at x0 as the vector whose
coordinates are the partial derivatives of f :
∇f (x0) =
(︃∂f (x0)
∂x1
, ∂f (x0)
∂x2
, . . . , ∂f (x0)
∂xk
)︃
Example: Consider f : R2 →R, (x, y) ↦→xy.
The gradient of f at (x, y) is ∇f (x, y) = (y, x).
The gradient of f at (3, −1) is ∇f (3, −1) = (−1, 3).
Theorem
Let D ⊆Rk be open. If f : D →R is differentiable (i.e., has a total derivative) at x0, then the
total derivative of f at x0 is equal to the gradient of f at x0
Df (x0) = ∇f (x0)
ECON 2050 – Basic Real Analysis III
22 / 31
```

## PDF page 23

```text
Tangent hyperplanes
We now can also determine tangent hyperplanes and estimate changes to values of
differentiable functions f :
Suppose D ⊆Rk is open and f : D →R differentiable at x0. Then Df (x0) = ∇f (x0) and
the tangent hyperplane to f at x0 is an affine function
g : Rk →R, x ↦→f (x0) + ∇f (x0)(x −x0)
Writing ∆y ≡f (x0 + dx) −f (x0) and dy ≡g(x0 + dx) −g(x0) we obtain
∆y ≈dy = ∇f (x0) · dx = ∂f (x0)
∂x1
dx1 + . . . + ∂f (x0)
∂xk
dxk
For dx sufficiently close to 0, the change in the tangent hyperplane approximates the
change in f .
ECON 2050 – Basic Real Analysis III
23 / 31
```

## PDF page 24

```text
(First-order) Taylor approximation
When x −x0 sufficiently small, f (x0) + ∇f (x0)(x −x0) can be used to approximate f (x):
f (x) = f (x0) + ∇f (x0)(x −x0) + O(x, x0)
where O(x, x0) becomes negligible when x is sufficiently close to x0.
Therefore, for x close to x0,
f (x) ≈f (x0) + ∇f (x0)(x −x0)
this is called the (first-order) Taylor approximation of f at the point x0.
ECON 2050 – Basic Real Analysis III
24 / 31
```

## PDF page 25

```text
(Total) differentiability vs. partial differentiability
Caution: In R1, by definition, f is differentiable in x0 if and only if f is partially differentiable
in x0. This is not true in Rk if k ≥2.
If D ⊆Rk is open and f : D →R is differentiable at x0 ∈D, then all partial derivatives
exist at x0. In other words, f is partially differentiable at x0.
However, the converse is not true: If f is partially differentiable at x0 ∈D, f is not
necessarily (totally) differentiable at x0.
ECON 2050 – Basic Real Analysis III
25 / 31
```

## PDF page 26

```text
Example:
All partial derivatives of
f : R2 →R, (x1, x2) ↦→
{︄x2
1 x2
x2
1 +x2
2
if (x1, x2) ̸= (0, 0)
0
if (x1, x2) = (0, 0)
at the point (0, 0) exist, but f is not differentiable at (0, 0).
ECON 2050 – Basic Real Analysis III
26 / 31
```

## PDF page 27

```text
If it exists, the derivative of f at (0, 0) is given by (a1, a2) such that:
lim
n→∞
|f (x1n, x2n) −f (0, 0) −a1x1n −a2x2n|
√︂
x2
1n + x2
2n
= 0
or,
lim
n→∞
⃓⃓⃓⃓⃓
x2
1x2
x2
1n + x2
2n
−a1x1n −a2x2n
⃓⃓⃓⃓⃓·
1
√︂
x2
1n + x2
2n
= 0
1. Take the sequence (x1n, x2n) =
(︁1
n, 1
n
)︁
. Then the above limit becomes:
lim
n→∞
⃓⃓⃓⃓⃓
1
n3
2
n2
−a1
n −a2
n
⃓⃓⃓⃓⃓
1
√
2
n
= lim
n→∞
⃓⃓⃓⃓
1
2
√
2
−a1 + a2
√
2
⃓⃓⃓⃓= 0
which is satisfied if and only if
a1 + a2 = 1
2
(1)
ECON 2050 – Basic Real Analysis III
27 / 31
```

## PDF page 28

```text
2. Take the sequence (x1n, x2n) =
(︁1
n2 , 1
n
)︁
. Then the above limit becomes:
lim
n→∞
⃓⃓⃓⃓⃓
1
n5
1
n4 + 1
n2
−a1
n2 −a2
n
⃓⃓⃓⃓⃓
1
√︂
1
n4 + 1
n2
= lim
n→∞
⃓⃓⃓⃓
1
n + n3 −a1
n2 −a2
n
⃓⃓⃓⃓
n2
√
1 + n2 = 0
which is satisfied if and only if
a2 = 0
(2)
ECON 2050 – Basic Real Analysis III
28 / 31
```

## PDF page 29

```text
3. Take the sequence (x1n, x2n) =
(︁1
n, 1
n2
)︁
. Then the above limit becomes:
lim
n→∞
⃓⃓⃓⃓⃓
1
n4
1
n2 + 1
n4
−a1
n −a2
n2
⃓⃓⃓⃓⃓
1
√︂
1
n2 + 1
n4
= lim
n→∞
⃓⃓⃓⃓
1
n2 + 1 −a1
n −a2
n2
⃓⃓⃓⃓
n2
√
n2 + 1
= 0
which is satisfied if and only if
a1 = 0
(3)
Since there is no a1, a2 satisfying all equations (1)-(3), the function f is not differentiable at
(0, 0).
ECON 2050 – Basic Real Analysis III
29 / 31
```

## PDF page 30

```text
We now check that all partial derivatives exist. Recall the definition of partial derivative with
respect to x1 at x0:
lim
n→∞
f (x10 + hn, x20) −f (x10, x20)
hn
.
For x0 = (0, 0), this simplifies to
lim
n→∞
f (hn, 0) −f (0, 0)
hn
;
and the given f this becomes (recalling that the sequence (hn) is such that hn →0 and hn ̸= 0
for all n)
lim
n→∞
(hn)2·0
(hn)2+02 −0
hn
= 0.
An analogous argument shows that the definition of partial derivative with respect to x2 at x0
also exists and equals zero.
ECON 2050 – Basic Real Analysis III
30 / 31
```

## PDF page 31

```text
So we have to be careful: Blindly computing the partial derivatives and assuming that the
corresponding tangent hyperplane approximates f well can backfire!
However:
Theorem
If D ⊆Rk is open and f : D →R is continuously partially differentiable, then f is continuously
differentiable.
Also note that if f has a tangent hyperplane at a point, then f is continuous at that point:
Theorem
If D ⊆Rk is open and f : D →R is differentiable at a point x0 ∈D, then f is continuous at
x0.
ECON 2050 – Basic Real Analysis III
31 / 31
```
