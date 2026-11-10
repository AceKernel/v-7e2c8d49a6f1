# Lecture 2: automatic text transcript

Original: [Lecture 2 PDF](lecture-02.pdf). Topic: Continuity and differentiation.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050 – Mathematical Economics
Basic Real Analysis II
ECON 2050 – Basic Real Analysis II
1 / 33
```

## PDF page 2

```text
Functions of several variables (SB Chapter 13.1)
Now we turn our attention to “functions of several variables” — functions
f : D →Rm
whose domain is some D ⊆Rk. Often, f is real-valued (i.e. m = 1). Utility, demand,
production, cost and profit functions are all examples (for concrete examples, see SB pp.
274-276).
Some authors just write
f (x) = x2
instead of
f : R →R, x ↦→x2
etc.,
and take D as the largest set of points for which f is well-defined.
ECON 2050 – Basic Real Analysis II
2 / 33
```

## PDF page 3

```text
Examples:
f (x1, x2) =
1
x1−x2 has the domain D = {(x1, x2) ∈R2 : x1 ̸= x2}.
f (x1, x2) = 1
x1 has the domain D = {(x1, x2) ∈R2 : x1 ̸= 0}.
f (x1, x2) = ln(x1 + x2) has the domain D = {(x1, x2) ∈R2 : x1 + x2 > 0}.
f (x) = √x has the domain D = {x ∈R : x ≥0}.
ECON 2050 – Basic Real Analysis II
3 / 33
```

## PDF page 4

```text
Graphs and level curves of functions (SB Chapter 13.2)
Graphing a function is often very useful if D ⊆R2.
3-dimensional plot: graph of f
Recall: graph of f = {(x, y) ∈D × R ⊆R3 : y = f (x)}
2-dimensional plot: contour plot of f
The level curve (or contour line) of level c of f : D ⊆R2 →R is the set of points
{x ∈D : f (x) = c}.
A contour plot usually shows the level curves for several c.
ECON 2050 – Basic Real Analysis II
4 / 33
```

## PDF page 5

```text
Example. Below the graph of the function f : R2 →R, (x1, x2) ↦→x2
1 + x2
2.
ECON 2050 – Basic Real Analysis II
5 / 33
```

## PDF page 6

```text
The level curve of level 8 of f is the result of first intersecting the graph of f with the
horizontal plane y = 8 and projecting the intersection to the x1-x2-plane:
ECON 2050 – Basic Real Analysis II
6 / 33
```

## PDF page 7

```text
We obtain a contour plot by drawing several level curves of f .
ECON 2050 – Basic Real Analysis II
7 / 33
```

## PDF page 8

```text
Below a contour plot and, again, the graph of f .
ECON 2050 – Basic Real Analysis II
8 / 33
```

## PDF page 9

```text
If you have taken intermediate microeconomics, you have already encountered level curves:
Level curve of a utility function u : R2
+ →R =
indifference curve
.
Example. Cobb-Douglas utility function u : R2
+ →R, (x1, x2) ↦→x0.5
1 x0.5
2
x1
x2
Level curve of a production function F : R2
+ →R =
isoquant
.
ECON 2050 – Basic Real Analysis II
9 / 33
```

## PDF page 10

```text
Continuity (SB Chapter 13.4)
Intuitively, a function of one variable is continuous if its graph has no breaks.
x
y
x0
A continuous function
x
y
x0
A discontinuous function
ECON 2050 – Basic Real Analysis II
10 / 33
```

## PDF page 11

```text
Formally and more generally,
Definition
Let D ⊆Rk. A function f : D →Rm is
continuous at x = (x1, x2, ..., xk) ∈D if for every sequence (xn) in D that converges to
x, the sequence (f (xn)) in Rm converges to f (x).
discontinuous at x otherwise.
continuous if it is continuous at x for all x ∈D.
ECON 2050 – Basic Real Analysis II
11 / 33
```

## PDF page 12

```text
Why do we care?
For example:
Consumer theory predicts that the consumer will choose a (utility) maximizing bundle.
Hence it is important to know that there actually is a maximizing bundle. Otherwise,
what does the theory tell us?
The following theorem guarantees that every continuous utility function has a maximum
in a budget set. Hence with continuity, we are fine!
(Recall from the discussion in the previous lecture that budget sets are compact sets.)
Theorem (Extreme Value Theorem)
Let D ⊆Rk be compact and f : D →R be continuous. Then f has a global maximum, that
is, there exists a x∗∈D such that f (x∗) ≥f (x) for all x ∈D.
This result will be discussed in detail when we discuss optimization.
ECON 2050 – Basic Real Analysis II
12 / 33
```

## PDF page 13

```text
Proving continuity of a function at x directly may not be too straightforward as it requires
checking if f (xn) →f (x) for every (xn) that converges to x.
However, if we find a single xn →x such that f (xn) doesn’t converge to f (x), then we know
that f is discontinuous at x.
ECON 2050 – Basic Real Analysis II
13 / 33
```

## PDF page 14

```text
Example: Consider the function f : R2 →R with
f (x1, x2) =
{︄x1x2
x2
1 +x2
2
if (x1, x2) ̸= (0, 0)
0
if (x1, x2) = (0, 0)
We show that it is discontinuous at (0, 0).
The sequence (ˆxn) = ( 1
n, 0) converges to (0, 0). Since
f (ˆxn) = f
(︃1
n, 0
)︃
=
1
n · 0
(︁1
n
)︁2 + 02 = 0,
∀n,
the sequence (f (ˆxn)) converges to 0.
(˜xn) = ( 1
n, 1
n) also converges to (0, 0), but f (˜xn) →1
2 as
f (˜xn) = f
(︃1
n, 1
n
)︃
=
1
n · 1
n
(︁1
n
)︁2 +
(︁1
n
)︁2 = 1
2,
∀n.
Therefore, we cannot have have f (xn) →0 for all (xn) such that xn →(0, 0).
ECON 2050 – Basic Real Analysis II
14 / 33
```

## PDF page 15

```text
Let D ⊆Rk and E ⊆Rk. For f : D →R and g : E →R, define the following functions:
f + g : D ∩E →R, x ↦→f (x) + g(x)
f −g : D ∩E →R, x ↦→f (x) −g(x)
f · g : D ∩E →R, x ↦→f (x)g(x)
f /g : D ∩{x ∈E : g(x) ̸= 0} →R, x ↦→f (x)
g(x)
ECON 2050 – Basic Real Analysis II
15 / 33
```

## PDF page 16

```text
The following theorem helps to show that functions are continuous.
Theorem
If f : D →R and g : E →R are continuous at x ∈D ∩E, then f + g, f −g, f · g, and f /g
(if g(x) ̸= 0) are all continuous at x.
Proof for f + g: Let (xn) be a sequence converging to x.
Because both f and g are continuous, f (xn) converges to f (x), and g(xn) converges to
g(x).
By a theorem from the previous lecture, f (xn) + g(xn) converges to f (x) + g(x).
By definition, f + g is also continuous at x.
The proof for f −g is analogous
ECON 2050 – Basic Real Analysis II
16 / 33
```

## PDF page 17

```text
Theorem
Let D ⊆Rk and f = (f1, . . . , fm) : D →Rm. Then f is continuous at x ∈D if and only if for
every i = 1, . . . , m, fi is continuous at x ∈D.
This is because a theorem from the previous lecture (Slide 23) indicates that f (xn) →f (x∗) if
and only if fi(xn) →fi(x∗) for each i = 1, . . . , k.
Theorem
For every i = 1, . . . , k, the i-th projection pri : Rk →R, x ↦→pri(x) = xi is a continuous
function.
This is because if xn →x∗, then for any i = 1, . . . , k, xin →x∗
i , where xin and x∗
i are the i-th
coordinate of xn and x∗, respectively. Alternatively, one may also consider f : Rm →Rm given
by f (x) = x, and then use the theorem above.
ECON 2050 – Basic Real Analysis II
17 / 33
```

## PDF page 18

```text
Let D ⊆Rk and f : D →Rm. Let g : E →Rl, where f (D) ⊆E. Then we define the
composition of f with g as
g ◦f : D →Rl, x ↦→g(f (x))
Theorem
Let D ⊆Rk and f : D →Rm be continuous at x ∈D. Let g : E →Rl be continuous at
f (x) ∈E, where f (D) ⊆E. Then g ◦f : D →Rl is continuous at x.
Proof: Let (xn) be an arbitrary sequence contained in D converging to x.
By the continuity of f at x, f (xn) →f (x).
By the continuity of g at f (x), g(f (xn)) →g(f (x)).
This implies, by definition, that g ◦f is continuous at x.
The theorems we just discussed can be very powerful in proving continuity.
ECON 2050 – Basic Real Analysis II
18 / 33
```

## PDF page 19

```text
Example: f : R2 →R, x ↦→x2
1 + x2
2 is continuous.
Proof: The trick is to observe that f = (pr1)2 + (pr2)2:
Recall that pri : R2 →R, x ↦→pri(x) = xi
Hence pri · pri, or, more succinctly, (pri)2 is the function
(pri)2 : R2 →R, x ↦→x2
i ,
and
(pr1)2 + (pr2)2 : R2 →R, x ↦→((pr1)2(x) + (pr2)2(x)) = x2
1 + x2
2.
Therefore, (pr1)2 + (pr2)2 equals f . By the previous theorems,
pri is continuous, and therefore,
pr2
i is continuous, and therefore,
(pr1)2 + (pr2)2 is continuous (that is, f is continuous!)
Alternatively, we can prove that f : R2 →R, x ↦→x2
1 + x2
2 is continuous by realizing that
f = g ◦pr1 + g ◦pr2 for g : R →R, x ↦→x2.
ECON 2050 – Basic Real Analysis II
19 / 33
```

## PDF page 20

```text
Exercises:
Let D = R3\{(x, y, z) ∈R3 : x + y + z = 0}. Then
ˆf : D →R, (x, y, z) ↦→
xyz
x + y + z
is continuous.
Proof:
ˆf =
pr1 · pr2 · pr3
pr1 + pr2 + pr3
˜f : R2\{(0, 0)} →R, (x, y) ↦→ln(x2 + y2) is continuous.
Proof:
˜f = ln ◦f ,
where f : R2\{(0, 0)} →R, x ↦→x2
1 + x2
2, and both f (see above) and ln are continuous.
ECON 2050 – Basic Real Analysis II
20 / 33
```

## PDF page 21

```text
Linear functions (SB pp. 287-289)
The inner product (or dot product) on Rk of x ∈Rk and y ∈Rk is
x · y =
k
∑︂
i=1
xiyi = x1y1 + x2y2 + . . . + xkyk.
A function f : Rk →R is linear if and only if there exists a ∈Rk such that
f (x) = a · x (=
k
∑︂
i=1
aixi)
for all x ∈Rk.
When k = 1, a linear function satisfies f (x) = ax for some a ∈R, where a is the slope (rise
over run) of f .
ECON 2050 – Basic Real Analysis II
21 / 33
```

## PDF page 22

```text
Affine functions (SB p. 292)
A function f : Rk →R is affine if there exist a ∈Rk and b ∈R such that f (x) = a · x + b for
all x ∈Rk.
For all x0, x ∈Rk and every affine f : Rk →R, x ↦→a · x + b,
f (x) −f (x0) = a · x + b −(a · x0 + b)
= a · x + b −a · x0 −b
= a · x −a · x0
= a · (x −x0)
When k = 1, an affine function satisfies f (x) = ax + b for some a, b ∈R.
ECON 2050 – Basic Real Analysis II
22 / 33
```

## PDF page 23

```text
Letting dx ≡x −x0 and dy ≡f (x) −f (x0), the last equation becomes
dy = a · dx (=
k
∑︂
i=1
ai dxi).
Therefore, if f is affine, the change dy in the value of f is a linear function of the change dx
in its variables.
Exercise: Suppose f (x1, x2) = 0.5x1 + 1.25x2 + 1.75.
How does the value of f change if we move from x0 = (1, 0.5) by dx = (dx1, dx2) = (1.5, 1) to
x = x0 + dx = (2.5, 1.5)?
It changes by
dy = 0.5dx1 + 1.25dx2 = 0.5 · 1.5 + 1.25 · 1 = 2
ECON 2050 – Basic Real Analysis II
23 / 33
```

## PDF page 24

```text
Note that we can “decompose” the change to f from moving from x0 = (1, 0.5) to
x0 + dx = (2.5, 1.5) into
the change from moving just in the x1 direction (by dx1 = 2.5 −1 = 1.5),
dy1 = 0.5dx1 = 0.5 · 1.5 = 0.75,
plus
the change from moving just in the x2 direction (by dx2 = 1.5 −0.5 = 1),
dy2 = 1.25dx2 = 1.25 · 1 = 1.25.
The total change to f is
dy = dy1 + dy2 = 2
ECON 2050 – Basic Real Analysis II
24 / 33
```

## PDF page 25

```text
An analogous decomposition holds for changes in the value of affine functions in general:
Recall that
dy = a · dx (=
k
∑︂
i=1
ai dxi)
if we move by dx.
If we just move by dxi (that is, just in the xi direction), from any x0 to
x0 + (0, . . . , 0, dxi, 0, . . . , 0) = (x0,1, . . . , x0,i + dxi, . . . , x0,k),
then
dyi = f (x0 + (0, . . . , 0, dxi, 0, . . . , 0)) −f (x0) = ai dxi
ECON 2050 – Basic Real Analysis II
25 / 33
```

## PDF page 26

```text
Hence we can write
dy =
k
∑︂
i=1
dyi
The change from moving from x0 to x0 + dx = x0 + d(x1, . . . , xk) equals the sum of the
changes of
just moving in the x1 direction, by dx1, and
just moving in the x2 direction, by dx2, and
. . .
just moving in the xk direction, by dxk.
ECON 2050 – Basic Real Analysis II
26 / 33
```

## PDF page 27

```text
Differentiability: Function of one variable (a review)
x
y
f
tangent line g : R →R
x ↦→f (x0) + f ′(x0)(x −x0)
x0
f (x0)
x0 + dx
f (x0 + dx)
g(x0 + dx)
approx. error
dy
∆y
dx
ECON 2050 – Basic Real Analysis II
27 / 33
```

## PDF page 28

```text
In the previous slide:
around x0, f is approximated by the affine function g tangent to f at x0
f ′(x0) is the slope of the tangent line g
∆y = f (x0 + dx) −f (x0) = actual change in y due to change dx in x
dy = g(x0 + dx) −g(x0) = f ′(x0)dx = approximate change in y due to change dx in x;
note that dy is a linear function of dx
if dx is “small,”
∆y ≈dy = f ′(x0)dx,
and f ′(x0) measures how much the change dx in x affects y = f (x)
as dx approaches 0, the approximation error also goes to 0
ECON 2050 – Basic Real Analysis II
28 / 33
```

## PDF page 29

```text
The formal definition of differentiability is as follows:
Definition
Let D ⊆R be open. The function f : D →R is differentiable at x0 ∈D if there exists
f ′(x0) ∈R such that
f ′(x0) = lim
n→∞
f (x0 + hn) −f (x0)
hn
for all sequences (hn) with hn →0 and hn ̸= 0 for all n. In this case, f ′(x0) is called the
derivative of f at x0.
It is useful to rephrase this definition a bit:
f : D →R is differentiable at x0 if and only if there exists a ∈R such that
lim
n→∞
f (x0 + hn) −f (x0) −ahn
hn
= 0
for all sequences (hn) with hn →0 and hn ̸= 0 for all n. In this case, a = f ′(x0).
ECON 2050 – Basic Real Analysis II
29 / 33
```

## PDF page 30

```text
f : D →R is differentiable at x0 if and only if there exists a ∈R such that
lim
n→∞
f (xn) −f (x0) −a(xn −x0)
xn −x0
= 0
for all sequences (xn) with xn →x0 and xn ̸= x0 for all n. In this case, a = f ′(x0).
If f : D →R is differentiable at x0, then the tangent line of f at x0, given by
g : R →R, x ↦→f (x0) + f ′(x0)(x −x0)
is an affine function that approximates f around x0 in the sense that whenever |x −x0| is
sufficiently small, the “approximation error” |f (x) −g(x)| is negligible.
ECON 2050 – Basic Real Analysis II
30 / 33
```

## PDF page 31

```text
Example: Let f : R →R be given by f (x) = x2.
By definition, fix any x ∈R and hn →0 (but hn ̸= 0 for all n), we have
f (x + hn) −f (x)
hn
= (x + hn)2 −x2
hn
= x2 + 2xhn + h2
n −x2
hn
= 2x + hn
But then f ′(x) = limn→∞(2x + hn) = 2x.
ECON 2050 – Basic Real Analysis II
31 / 33
```

## PDF page 32

```text
Example: Let f : R →R+ be given by f (x) = |x|.
This function is not differentiable at x0 = 0:
Consider the sequence (1/n),
f (0 + 1/n) −f (0)
1/n
= |0 + 1/n| −|0|
1/n
= 1/n
1/n = 1.
On the other hand, consider the sequence (−1/n),
f (0 + (−1/n)) −f (0)
−1/n
= |0 −1/n| −|0|
−1/n
= 1/n
−1/n = −1.
ECON 2050 – Basic Real Analysis II
32 / 33
```

## PDF page 33

```text
Observe that f (x) = |x| is continuous because its graph has no breaks:
x
y
−3
−2
−1
1
2
3
1
2
3
In fact:
Theorem
If D ⊆R is open and f : D →R is differentiable at a point x0 ∈D, then f is continuous at x0.
ECON 2050 – Basic Real Analysis II
33 / 33
```
