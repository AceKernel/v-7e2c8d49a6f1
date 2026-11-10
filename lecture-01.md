# Lecture 1: automatic text transcript

Original: [Lecture 1 PDF](lecture-01.pdf). Topic: Norms, sequences, topology and compactness.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050 – Mathematical Economics
Basic Real Analysis I
ECON 2050 – Basic Real Analysis I
1 / 30
```

## PDF page 2

```text
The space we work in
This course assumes basic familiarity of the set of real numbers, or the real line, denoted by R.
The distance between x ∈R and y ∈R is the absolute value of x −y, that is, |x −y|. If
this distance is small, then x and y are “close” to each other.
R
-3
-2
-1
0
1
2
3
4
x = 2.5
y
x −y = −1.5
|2.5 −4| = 1.5
In particular, the distance between x ∈R and 0, |x| = |x −0|, measures the “length” of x.
R
-3
-2
-1
0
1
2
3
4
2.5
|2.5 −0| = |2.5|
ECON 2050 – Basic Real Analysis I
2 / 30
```

## PDF page 3

```text
More generally, we will work with the set of all m-tuples of real numbers, denoted by Rm,
where m is a positive integer.
A point in Rm can be written as x = (x1, . . . , xm), where xi is its i-th coordinate.
When m = 1, we get the familiar real line R.
x1
x2
x = (3, 4)
ECON 2050 – Basic Real Analysis I
3 / 30
```

## PDF page 4

```text
We also generalize the ideas of distance and length to Rm with m > 1: as in R, in Rm the
norm (generalizing the absolute value) of x = (x1, . . . , xm) ∈Rm is the “length” of x, or the
distance between x and 0; denote it by ∥x∥.
x = (x1, x2)
∥x∥
x2
x1
By Pythagoras’ Theorem, ∥x∥2 = x2
1 + x2
2, or
∥x∥=
√︂
x2
1 + x2
2
ECON 2050 – Basic Real Analysis I
4 / 30
```

## PDF page 5

```text
More generally (for arbitrary positive integer m):
Definition
The norm of x = (x1, . . . , xm) ∈Rm is
∥x∥=
√︂
x2
1 + x2
2 + ... + x2m
The distance between x ∈Rm and y ∈Rm is
∥x −y∥= ∥(x1 −y1, x2 −y2, . . . , xm −ym)∥
=
√︂
(x1 −y1)2 + (x2 −y2)2 + . . . + (xm −ym)2
Rm is sometimes called an Euclidean space.
This definition generalizes our earlier definitions:
▶The norm of x1 ∈R (= R1) is ∥x1∥=
√︁
x2
1 = |x1|
▶The norm of a point x = (x1, x2) ∈R2 in a plane is ∥x∥=
√︁
x2
1 + x2
2
ECON 2050 – Basic Real Analysis I
5 / 30
```

## PDF page 6

```text
Functions (SB p. 273)
Definition
A function f from a set X to a set Y is a rule that assigns to each element of X exactly one
element of Y . We write f : X →Y or f : X →Y , x ↦→f (x).
the domain of f is the set X
the codomain (or target space in SB) of f is the set Y
the image of x under f , written f (x), is the element y ∈Y which f assigns to x ∈X
the range or image of f is the set f (X) = {y ∈Y : y = f (x) for some x ∈X}
the graph of f is the set {(x, y) ∈X × Y : y = f (x)}
ECON 2050 – Basic Real Analysis I
6 / 30
```

## PDF page 7

```text
Example: X = [0, 4], Y = [0.5, 4.5], f : X →Y as shown below
x
y
1
1
2
2
3
3
4
4
graph of f
x
f (x)
codomain of f
domain of f
image of f
(= [1, 3])
ECON 2050 – Basic Real Analysis I
7 / 30
```

## PDF page 8

```text
Sequences (SB Section 12.1 & 12.2)
Definition
A sequence (in X) is a function f : N →X.
N = {1, 2, 3, . . .} = set of natural numbers
we are interested in the cases X = R and X = Rm where m ∈N
it is common to write (xn) or (xn)n∈N or (xn)∞
n=1 or (x1, x2, x3, . . .) for f , where
xn ≡f (n)
Example: ( 1
n)n∈N denotes f : N →R, n ↦→1
n
SB write {xn} or {xn}n∈N or {xn}∞
n=1 or {x1, x2, x3, . . .} for f
ECON 2050 – Basic Real Analysis I
8 / 30
```

## PDF page 9

```text
Example: Below, we illustrate the first elements of the sequence f : N →R given by
(1
1, 1, 1
2, 2, 1
3, 3, . . .)
O
N
R
1
2
3
4
5
6
7
8
9
1
2
3
4
ECON 2050 – Basic Real Analysis I
9 / 30
```

## PDF page 10

```text
Often, we want to figure out where a sequence “tends to” as the index n ∈N becomes “large”
(i.e., goes to +∞)
Example: Interest rate = 3.5% (both for saving and borrowing). Your bank offers to pay you
(and your offspring) $1000/year for n years. How much should you maximally pay for this?
If n = 1, then the maximum you should pay is:
PV1 = 1000
If n = 2, then the maximum you should pay is:
PV2 = 1000 + 1000
1.035 ≈1000 + 966 = 1966
More generally,
PVn = 1000 + 1000
1.0351 + . . . +
1000
1.035n−1
=
n−1
∑︂
k=0
1000
1.035k = 1000 ·
k−1
∑︂
k=0
(︃
1
1.035
)︃k
ECON 2050 – Basic Real Analysis I
10 / 30
```

## PDF page 11

```text
This defines a sequence (PVn)∞
n=1; up to rounding:
(PVn)∞
n=1 = (1000, 1966, 2900, 3802, 4673, . . .)
Where does (PVn)∞
n=1 “tend to” as n →∞?
PVn = 1000
+ 1000
1.0351 + . . . . . .+
1000
1.035n−2 +
1000
1.035n−1
(1)
1
1.035PVn = 1000
1.0351 + 1000
1.0352 + . . . . . .+
1000
1.035n−1 + 1000
1.035n
(2)
(1) −(2) :
(︃
1 −
1
1.035
)︃
PVn = 1000 −1000
1.035n .
Therefore:
PVn = 1000 −
1000
1.035n
1 −
1
1.035
≈29571 −
1000
1.035n
1 −
1
1.035
(≈29571 for n large)
ECON 2050 – Basic Real Analysis I
11 / 30
```

## PDF page 12

```text
Definition
Let (xn)n∈N be a sequence with codomain R. We say that (xn) converges to x∗or that x∗is
the limit of (xn)n∈N, and write limn→∞xn = x∗or xn →x∗, if
∀ε > 0 ∃N ∈N s.t. ∀n ≥N : |xn −x∗| < ε.
If (xn)n∈N does not converge to any x∗∈R we say that (xn)n∈N diverges.
ECON 2050 – Basic Real Analysis I
12 / 30
```

## PDF page 13

```text
Example
Consider the sequence ( 1
n)n∈N, we also have lim
n→∞
1
n = 0
n
(xn)
1
1
2
0.5
3
0.333333
4
0.25
5
0.2
6
0.166667
7
0.142857
8
0.125
9
0.111111
10
0.1
11
0.090909
12
0.083333
13
0.076923
ECON 2050 – Basic Real Analysis I
13 / 30
```

## PDF page 14

```text
Suppose ϵ = 0.1, what is the appropriate N?
Intuitively, we can see that when N = 11, all other n > 11, the distance between xn and
x∗is less than ϵ
But how do we generalise this for any ϵ > 0?
ECON 2050 – Basic Real Analysis I
14 / 30
```

## PDF page 15

```text
The idea of convergence is that the tail of a sequence approximates its limit to any desired
degree of accuracy.
Some initial finitely many terms of the sequence may be quite apart from its limit, but
eventually all terms of the sequence accumulates around this limit.
To see this, consider a sequence (xn) defined as
xn =
{︃n
if n ≤100;
1
n−100
if n > 100.
To show that limn→∞xn = 0, we need to pick N large enough; in fact, we need to pick
N > (1/ε) + 100.
So although real sequences (1/n) and xn appear to be quite different in their first 100
terms, they have the same long-run behavior: they both converge to 0.
That is, the initial terms of the sequence have no say on the behavior of the tail of the
sequence.
ECON 2050 – Basic Real Analysis I
15 / 30
```

## PDF page 16

```text
Sequences in Rm
Sometimes, we want to consider sequences with codomain Rm.
Example: Every second, we observe Ann’s x1 and x2 coordinates (her position on a plane). At
time t, her position is
xt = (x1,t, x2,t) =
(︃30
t sin
(︃30
t
)︃
, 30
t cos
(︃30
t
)︃)︃
Will Ann’s position “converge” to some location? That is, will the sequence (xt)t∈N converge?
Convention: We use x ∈Rm and (x1, . . . , xm) ∈Rm interchangeably.
ECON 2050 – Basic Real Analysis I
16 / 30
```

## PDF page 17

```text
Below a picture of a few elements of (xt)t∈N:
R
R
x2
x3
x4
x5
x6
x7 x8x9
It appears as if xt →(0, 0): Ann gets closer and closer to (0, 0). To verify this, let’s formalize
the notion of convergence in Rm.
ECON 2050 – Basic Real Analysis I
17 / 30
```

## PDF page 18

```text
Definition
Let (xn)n∈N be a sequence with codomain Rm. We say that (xn) converges to x∗or that x∗
is the limit of (xn)n∈N, and write limn→∞xn = x∗or xn →x∗, if
∀ε > 0 ∃N ∈N s.t. ∀n ≥N : ∥xn −x∗∥< ε.
If (xn)n∈N does not converge to any x∗∈Rm we say that (xn)n∈N diverges.
We can rewrite this definition using the notion of open balls:
Definition
The open ball Br(x) with radius r > 0 and center x ∈Rm is the set of points y ∈Rm with
distance less than r from x,
Br(x) = {y ∈Rm : ∥y −x∥< r} .
A sequence (xn)n∈N with codomain Rm converges to x∗if and only if
∀ε > 0 ∃N ∈N s.t. ∀n ≥N : xn ∈Bε(x∗).
ECON 2050 – Basic Real Analysis I
18 / 30
```

## PDF page 19

```text
In R (m = 1), an open ball is an open interval.
R
-1
0
1
2
3
4
5
6
B1.5(3) = { y ∈R : |y −3| < 1.5} = { y ∈R : 1.5 < y < 4.5} = (1.5, 4.5)
Note that the empty circles at the endpoints of the interval (1.5, 4.5) indicate that 1.5 and 4.5
are not in B1.5(3).)
ECON 2050 – Basic Real Analysis I
19 / 30
```

## PDF page 20

```text
In R2 (m = 2), the open ball Br(x1, x2) consists of all points in the circle with radius r
around (x1, x2), excluding the circle’s border.
Convention: When we draw sets, solid lines are part of the set, dotted lines are not.
R
R
1
2
3
4
5
6
7
8
1
2
3
1
B1(1.5, 1.5)
1
circle around (4, 1.5)
1
B1(6.5, 1.5) ∪
circle around (6.5, 1.5)
ECON 2050 – Basic Real Analysis I
20 / 30
```

## PDF page 21

```text
Theorem (compare SB Thm 12.1)
A sequence can have at most one limit.
Intuition: a sequence cannot get arbitrarily close and stay arbitrarily close to two different
points.
Proof: See supplementary materials on Blackboard (ie: Logic.pdf)
ECON 2050 – Basic Real Analysis I
21 / 30
```

## PDF page 22

```text
Theorem
If limn→∞xn = x∗∈Rm and limn→∞yn = y ∗∈Rm and c ∈R, then
(a) limn→∞(xn + yn) = x∗+ y ∗.
(b) limn→∞cxn = cx∗.
We will only prove part (a) and leave part (b) as an exercise. To that end, recall for
a, b, c ∈Rm:
∥a −c∥≤∥a −b∥+ ∥b −c∥
(triangle inequality — see SB Thm 10.5).
a
b
c
∥a −b∥
∥b −c∥
∥a −c∥
ECON 2050 – Basic Real Analysis I
22 / 30
```

## PDF page 23

```text
Proof of part (a): Let ε > 0.
1 Since xn →x∗, ∃N1 ∈N such that ∥xn −x∗∥< ε/2 for all n ≥N1.
2 Since yn →y ∗, ∃N2 ∈N such that ∥yn −y ∗∥< ε/2 for all n ≥N2.
Therefore ∥xn −x∗∥< ε/2 and ∥yn −y ∗∥< ε/2 for all n ≥N ≡max{N1, N2}. Then for all
n ≥N,
∥(xn + yn)−(x∗+ y ∗)∥= ∥(xn −x∗) −(y ∗−yn)∥
≤∥(xn −x∗) −0∥+ ∥0 −(y ∗−yn)∥(by triangle inequality)
= ∥xn −x∗∥+ ∥yn −y ∗∥
< ε
2 + ε
2
= ε,
where 0 = (0, . . . , 0). Thus, (xn + yn) →(x∗+ y ∗).
ECON 2050 – Basic Real Analysis I
23 / 30
```

## PDF page 24

```text
Theorem
Let (xn)n∈N and (yn)n∈N be sequences with codomain R. If limn→∞xn = x∗∈R and
limn→∞yn = y∗∈R, then
(a) limn→∞(xn · yn) = x∗· y∗
(b) if there exists b ∈R such that xn ≤b for all n ∈N, then x∗≤b.
Proof of part (a) is left as an exercise. See SB Thm 12.3 if you are interested.
Proof of part (b): Suppose, toward a contradiction, that xn ≤b for all n ∈N, but x∗> b.
Choose ε so that 0 < ε < x∗−b (e.g., we can let ε = (x∗−b)/2). Then, b < x∗−ε.
Because xn →x∗, there exists N ∈N such that for all n ≥N,
xn ∈Bε(x∗) = (x∗−ε, x∗+ ε).
This implies that xn ≥b for all n ≥N, a contradiction.
ECON 2050 – Basic Real Analysis I
24 / 30
```

## PDF page 25

```text
Theorem (compare SB Thm 12.5)
Let (xn)n∈N be a sequence with codomain Rm. Then
lim
n→∞xn = x∗
if and only if
(︂
lim
n→∞xi,n = x∗
i for all i = 1, . . . , m
)︂
.
We can use this theorem to verify that “Ann converges to (0, 0)”:
We have
lim
t→∞x1,t = lim
t→∞
30
t sin
(︃30
t
)︃
= 0
We have
lim
t→∞x2,t = lim
t→∞
30
t cos
(︃30
t
)︃
= 0
Therefore,
lim
t→∞xt =
(︃30
t sin
(︃30
t
)︃
, 30
t cos
(︃30
t
)︃)︃
= (0, 0)
ECON 2050 – Basic Real Analysis I
25 / 30
```

## PDF page 26

```text
Open and closed sets (SB Section 12.3 & 12.4)
Definition
Consider a set S ⊆Rm. A point x = (x1, . . . , xm) ∈Rm is
an interior point of S if there exists an open ball centered at x contained entirely in S.
an exterior point of S if there is an open ball centered at x located entirely outside of S.
a boundary point of S if each open ball centered at x contains both a point in S and a
point outside of S.
Note that a boundary point of S does not have to belong to S.
S
d
boundary point (/∈S)
b
boundary point (∈S)
a
exterior point
c
interior point
ECON 2050 – Basic Real Analysis I
26 / 30
```

## PDF page 27

```text
These notions allow us to define two important “topological” properties of sets:
Definition
A set S ⊆Rm is
open if all of its points are interior points.
closed if it contains all of its boundary points.
Examples:
The set S1 =
{︁
(x, y) ∈R2 : (x −1)2 + (y −1)2 < 1
}︁
is
open .
More generally, open intervals in R and open balls in Rm are open (SB Thm 12.7).
The set S2 =
{︁
(x, y) ∈R2 : (x −1)2 + (y −1)2 ≤1
}︁
is
closed . Its boundary is formed
by the points of the set
S3 =
{︁
(x, y) ∈R2 : (x −1)2 + (y −1)2 = 1
}︁
⊆S2.
Any closed interval [a, b] ≡{x ∈R : a ≤x ≤b} is
closed , with boundary points a, b.
ECON 2050 – Basic Real Analysis I
27 / 30
```

## PDF page 28

```text
The set S3 =
{︁
(x, y) ∈R2 : x ≥0, y ≥0, x + 2y ≤3
}︁
is
closed .
x
y
x + 2y = 3
The interior of a set S ⊆Rm, denoted by int(S), is the set of all interior points of S.
A set S ⊆Rm is open if and only if S = int(S).
ECON 2050 – Basic Real Analysis I
28 / 30
```

## PDF page 29

```text
Note that some sets are neither open nor closed.
Example:
/∈S, boundary point
→S not closed
∈S, not an interior point
→S not open
S
ECON 2050 – Basic Real Analysis I
29 / 30
```

## PDF page 30

```text
Bounded and compact sets (SB Section 12.5)
Besides open and closed sets, compact sets play an important role:
Definition
A set S ⊆Rm is
bounded if
∃K > 0 such that ∀x ∈S : ∥x∥≤K
(i.e. if there is an open ball centered at 0 that contains S).
compact if it is closed and bounded.
Examples:
Any closed interval [a, b] is compact.
Let p1, p2 ≥0 be two prices and w ≥0 be a wealth level.
▶B1 = {(x1, x2) ∈R2 : p1x1 + p2x2 ≤w} is closed but not bounded.
▶The budget set B2 = {(x1, x2) ∈R2 : p1x1 + p2x2 ≤w, x1 ≥0, x2 ≥0} is closed and
bounded, and therefore compact.
ECON 2050 – Basic Real Analysis I
30 / 30
```
