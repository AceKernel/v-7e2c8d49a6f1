# Lecture 7: automatic text transcript

Original: [Lecture 7 PDF](lecture-07.pdf). Topic: Convexity and concavity.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050 – Mathematical Economics
Convexity
ECON 2050 – Convexity
1 / 30
```

## PDF page 2

```text
Convex combinations and line segments
Definition
A convex combination of two vectors x, y ∈Rn is any vector z ∈Rn such that
z = λx + (1 −λ)y,
for some λ such that 0 ≤λ ≤1.
Definition
The line segment [x, y] between x ∈Rn and y ∈Rn is the set of all convex combinations of
x and y. That is,
[x, y] = {z ∈Rn : z = λx + (1 −λ)y for some λ such that 0 ≤λ ≤1}
ECON 2050 – Convexity
2 / 30
```

## PDF page 3

```text
Examples:
[0, 1] = line segment between 0 and 1 = closed interval between 0 and 1
[(1, 0), (3, 4)] = {(x, y) : (x, y) = λ(1, 0) + (1 −λ)(3, 4), 0 ≤λ ≤1}
= line segment between (1, 0) and (3, 4).
If λ = 0 we are at (3, 4); if λ = 1 we are at (1, 0); if λ = 1
2 we are at the midpoint
(2, 2) = 1
2(1, 0) + 1
2(3, 4) of the segment.
Note that the set
{z ∈Rn : z = λx + (1 −λ)y for some λ ∈R}
= {z ∈Rn : z = y + λ(x −y) for some λ ∈R}
describes the straight line through the points x, y.
ECON 2050 – Convexity
3 / 30
```

## PDF page 4

```text
Convex sets
Definition
A set S ⊆Rn is convex if for every two points of the set the line segment between the two
points belongs to the set, that is, if
∀x, y ∈S : [x, y] ⊆S,
or, equivalently, if
∀x, y ∈S, ∀λ ∈[0, 1] : λx + (1 −λ)y ∈S
A convex set
A set that is not convex
ECON 2050 – Convexity
4 / 30
```

## PDF page 5

```text
Examples: Intervals and (more generally) balls are convex sets.
Exercise: Determine whether the following four sets (in grey) are convex.
convex
convex
not convex
not convex
ECON 2050 – Convexity
5 / 30
```

## PDF page 6

```text
Example: T =
{︁
(x, y) ∈R2 : x + 2y ≤3
}︁
is convex: Let (x′, y′), (x′′, y′′) ∈T and λ ∈[0, 1].
We need to show that
λ(x′, y′) + (1 −λ)(x′′, y′′) = (λx′ + (1 −λ)x′′, λy′ + (1 −λ)y′′) ∈T,
or, equivalently, that
(λx′ + (1 −λ)x′′) + 2(λy′ + (1 −λ)y′′) ≤3.
(1)
But (x′, y′) ∈T implies x′ + 2y′ ≤3 and thus
λ(x′ + 2y′) ≤3λ,
(2)
and (x′′, y′′) ∈T implies x′′ + 2y′′ ≤3 and thus
(1 −λ)(x′′ + 2y′′) ≤3(1 −λ).
(3)
Adding up the two inequalities (2) and (3), we obtain (1).
ECON 2050 – Convexity
6 / 30
```

## PDF page 7

```text
Proposition
Every intersection of convex sets is a convex set.
Proof:
Suppose Si for i ∈I, are convex sets (where I is some “index” set, e.g. I = {1, 2, 3}).
If x, y ∈⋂︁
i∈I Si then x, y ∈Si for every i ∈I.
For every i, since Si is convex, the line segment between x and y, [x, y], is contained in
Si.
Therefore, [x, y] belongs to the intersection ⋂︁
i∈I Si.
Example: S =
{︁
(x, y) ∈R2 : x + 2y ≤3, x ≥0, y ≥0
}︁
is convex because
S = T ∩{(x, y) ∈R2 : x ≥0} ∩{(x, y) ∈R2 : y ≥0},
where T =
{︁
(x, y) ∈R2 : x + 2y ≤3
}︁
, and it is not difficult to check that both
{(x, y) ∈R2 : x ≥0}, {(x, y) ∈R2 : y ≥0} are convex (exercises; use definition).
ECON 2050 – Convexity
7 / 30
```

## PDF page 8

```text
Warning: In general, the union of convex sets is not a convex set.
Exercise: Write down or draw two convex sets S and T whose union S ∪T is not convex.
S = {1} and T = {2} are convex, but S ∪T = {1, 2} is not convex.
S = [1, 2] and T = [3, 4] are convex, but S ∪T = [1, 2] ∪[3, 4] is not convex: x′ = 2 and
x′′ = 3 are contained in S ∪T, but (1/2)x′ + (1/2)x′′ = (1/2)2 + (1/2)3 = 2.5 /∈S ∪T
S = B1(1, 0) and T = B1(−1, 0) are convex but S ∪T is not convex.
(E.g. (1, 1
2) ∈S and (−1, 1
2) ∈T both belong to S ∪T, but the midpoint (0, 1
2) of the
line segment [(1, 1
2), (−1, 1
2)] does not belong to either of the two sets and, therefore, it
does not belong to the union of them.)
ECON 2050 – Convexity
8 / 30
```

## PDF page 9

```text
Convex and Concave Functions (SB Chapter 21.1)
Definition
Let S ⊆Rn be convex. A function f : S →R is convex (on S) if ∀x, y ∈S, ∀λ ∈[0, 1]
f (λx + (1 −λ)y) ≤λf (x) + (1 −λ)f (y).
The function is strictly convex (on S) if ∀x, y ∈S such that x ̸= y, ∀λ ∈(0, 1),
f (λx + (1 −λ)y) < λf (x) + (1 −λ)f (y).
A function is convex if for all x and y, the graph of the function over the line segment
between x and y lies below the line segment between the points (x, f (x)) and (y, f (y)).
ECON 2050 – Convexity
9 / 30
```

## PDF page 10

```text
A strictly convex function of one variable:
x
y
(1
)
x
y
λ
λ
+
−
λ
+
−λ
f(x)
(
)f(y)
1
λ
+
−λ
f( x
(
)y)
1
( )
f x
f(y)
ECON 2050 – Convexity
10 / 30
```

## PDF page 11

```text
Definition
Let S ⊆Rn be convex. A function f : S →R is concave (on S) if ∀x, y ∈S, ∀λ ∈[0, 1]
f (λx + (1 −λ)y) ≥λf (x) + (1 −λ)f (y).
The function is strictly concave (on S) if ∀x, y ∈S such that x ̸= y, ∀λ ∈(0, 1),
f (λx + (1 −λ)y) > λf (x) + (1 −λ)f (y).
A function is concave if for all x and y, the graph of the function over the line segment
between x and y lies above the line segment between the points (x, f (x)) and (y, f (y)).
ECON 2050 – Convexity
11 / 30
```

## PDF page 12

```text
A strictly concave function of one variable:
λ
+
−λ
f(x)
(
)f(y)
1
x
y
(1
)
x
y
λ
λ
+
−
λ
+
−λ
f( x
(
)y)
1
f(x)
f(y)
ECON 2050 – Convexity
12 / 30
```

## PDF page 13

```text
Examples:
f (x1, x2) = x1 + x2 is both convex and concave:
Let (x′
1, x′
2), (x′′
1 , x′′
2 ) ∈R2 and λ ∈[0, 1], then
f (λ(x′
1, x′
2) + (1 −λ)(x′′
1 , x′′
2 )) = f (λx′
1 + (1 −λ)x′′
1 , λx′
2 + (1 −λ)x′′
2 )
= λx′
1 + (1 −λ)x′′
1 + λx′
2 + (1 −λ)x′′
2
= λ(x′
1 + x′
2) + (1 −λ)(x′′
1 + x′′
2 )
= λf (x′
1, x′
2) + (1 −λ)f (x′′
1 , x′′
2 )
Thus f is both concave and convex, but neither strictly concave nor strictly convex.
More generally, every affine function f : Rn →R is both convex and concave (exercise).
f1(x) = x2 and f2(x) = ex are strictly convex, f3(x) = ln x and f4(x) = √x are strictly
concave.
ECON 2050 – Convexity
13 / 30
```

## PDF page 14

```text
Increasing and decreasing functions: A review
Definition
Let T be a nonempty subset of R. A function f : T →R is said to be
increasing if for any x, y ∈T, x ≥y implies f (x) ≥f (y);
strictly increasing if for any x, y ∈T, x > y implies f (x) > f (y);
decreasing if for any x, y ∈T, x ≥y implies f (x) ≤f (y); and
strictly decreasing if for any x, y ∈T, x > y implies f (x) < f (y).
We call a function that is either increasing or decreasing monotone.
It is not difficult to see that f is (strictly) decreasing if and only if −f is (strictly)
increasing.
ECON 2050 – Convexity
14 / 30
```

## PDF page 15

```text
Theorem
Let I be an open interval and f : I →R be differentiable, then
(1) f is increasing if and only if f ′ ≥0 on I;
(2) if f ′ > 0 on I, then f is strictly increasing;
(3) f is decreasing if and only if f ′ ≤0; and
(4) if f ′ < 0 on I, then f is strictly decreasing.
Note that the converse of parts (2) and (4) need not hold: suppose f (x) = x3, we have
f ′(0) = 0 but f is strictly increasing.
ECON 2050 – Convexity
15 / 30
```

## PDF page 16

```text
Differentiable convex/concave function of one variable: A review
Theorem
Let I be an open interval and f : I →R be differentiable, then
f is (strictly) convex if and only if f ′ is (strictly) increasing;
f is (strictly) concave if and only if f ′ is (strictly) decreasing.
Corollary
Let I be an open interval and f : I →R be differentiable, then
f is convex if and only if f ′′ ≥0, and if f ′′ > 0, f is strictly convex;
f is concave if and only if f ′′ ≤0, and if f ′′ < 0, f is strictly concave.
ECON 2050 – Convexity
16 / 30
```

## PDF page 17

```text
Properties of convex/concave functions
Theorem (SB Theorem 21.8)
Let S ⊆Rn be convex, and f1, f2, . . . , fk be functions from S to R. If f1, f2, ..., fk are convex
[concave], then for all α ∈Rk such that αi ≥0 for all i = 1, . . . , k,
α1f1 + α2f2 + ... + αkfk
is also convex [concave].
Proof: Follows directly from the definition of convex/concave functions. A good (finger)
exercise.
ECON 2050 – Convexity
17 / 30
```

## PDF page 18

```text
Theorem
Let S ⊆Rn be convex, and f is a function from S to R.
1 If f is convex [concave] then −f : S →R, x ↦→−f (x) is concave [convex].
2 If f is convex [concave] and g : R →R is a convex [concave] and increasing function,
then g ◦f is convex [concave].
Proof: Part 1 follows directly from the definition, because minus sign reverses inequalities; for
part 2, just apply the definition twice and use the fact that g is increasing to “pass” the
inequality.
Warning: If g is not increasing, part 2 need not be true. E.g.,
f (x) = x2, is convex; g(y) = −y is convex but not increasing.
But g ◦f : R →R, given by g(f (x)) = −x2 is not convex.
ECON 2050 – Convexity
18 / 30
```

## PDF page 19

```text
Examples:
f : R →R, x ↦→3x2 + 2x is convex because
▶f1 : R →R, x ↦→x2 is convex,
▶f2 : R →R, x ↦→x is convex, and
▶f = 3f1 + 2f2
g : R →R, x ↦→−x2 is concave because
▶f1 : R →R, x ↦→x2 is convex,
▶g = −f1
h : R2
++ →R, (x, y) ↦→√5x + 2y is concave because
▶f : R2
++ →R+, (x, y) ↦→5x + 2y is affine (and therefore concave),
▶g : R+ →R, x ↦→√x is concave and increasing, and
▶h = g ◦f
ECON 2050 – Convexity
19 / 30
```

## PDF page 20

```text
We defined when a function is convex, and when a set is convex.
To distinguish these concepts, we could say “function-convex” and “set-convex,” but
commonly both concepts are simply called “convex.”
The next proposition shows how “function-convexity” and “set-convexity” are related.
Definition
Let S ⊆Rn be convex, and f : S →R. The epigraph of f is the set
epi(f ) = {(x, y) ∈S × R : y ≥f (x)} ,
and the hypograph of f is the set
hyp(f ) = {(x, y) ∈S × R : y ≤f (x)} .
Intuitively, the epigraph (hypograph) of a function is the set of all points that lie on or above
(below) its graph.
ECON 2050 – Convexity
20 / 30
```

## PDF page 21

```text
Epigraph and hypograph of a function of one variable:
Hypograph
Epigraph
f(x)
ECON 2050 – Convexity
21 / 30
```

## PDF page 22

```text
Proposition
Let S ⊆Rn be convex. A function f : S →R is
concave if and only if its hypograph is a convex set.
convex if and only if its epigraph is a convex set.
Proof (first part): “⇒”: Suppose that f is concave. We want to show that hyp(f ) is a convex
set.
Let (x1, y1), (x2, y2) ∈hyp(f ), and λ ∈[0, 1]. We have to show that
λ(x1, y1) + (1 −λ)(x2, y2) ∈hyp(f ).
Since (x1, y1) ∈hyp(f ), y1 ≤f (x1) and thus
λy1 ≤λf (x1)
(4)
Since (x2, y2) ∈hyp(f ), y2 ≤f (x2) and thus
(1 −λ)y2 ≤(1 −λ)f (x2)
(5)
ECON 2050 – Convexity
22 / 30
```

## PDF page 23

```text
Thus
λy1 + (1 −λ)y2 ≤λf (x1) + (1 −λ)f (x2) ≤f (λx1 + (1 −λ)x2),
where the first inequality follows from adding up (4) and (5) and the second inequality holds
because f is concave. We conclude that
(λx1 + (1 −λ)x2, λy1 + (1 −λ)y2) = λ(x1, y1) + (1 −λ)(x2, y2) ∈hyp(f )
Therefore, hyp(f ) is convex.
ECON 2050 – Convexity
23 / 30
```

## PDF page 24

```text
“⇐”: Now suppose that hyp(f ) is convex. We want to show that f is concave.
Take x1, x2 ∈S and let λ ∈[0, 1]. We have to show that
λf (x1) + (1 −λ)f (x2) ≤f (λx1 + (1 −λ)x2).
Since x1, x2 ∈S, (x1, f (x1)), (x2, f (x2)) ∈hyp(f ). Because hyp(f ) is convex,
λ(x1,f (x1)) + (1 −λ)(x2, f (x2))
= (λx1 + (1 −λ)x2, λf (x1) + (1 −λ)f (x2)) ∈hyp(f )
Thus by the definition of a hypograph:
λf (x1) + (1 −λ)f (x2) ≤f (λx1 + (1 −λ)x2)
Therefore, f is concave.
ECON 2050 – Convexity
24 / 30
```

## PDF page 25

```text
Example: S =
{︁
(x, y, z) ∈R3 : x2 + y2 ≤1, z = 1
}︁
is convex, because
f (x, y) = x2 + y2 is convex (will be proved later);
thus epi(f ) =
{︁
(x, y, z) ∈R3 : z ≥x2 + y2}︁
is convex;
S = intersection of epi(f ) with the plane described by z = 1, which is also convex
Exercise: Prove that the set T =
{︁
(x, y) : y ≥x2}︁
is convex.
We know that g(x) = x2 is a convex function. Since T = epi(g), by the previous proposition,
T is a convex set.
ECON 2050 – Convexity
25 / 30
```

## PDF page 26

```text
First-order conditions for convexity/concavity
Theorem (compare SB Thm 21.2, 21.3)
If S ⊆Rn is open and convex and f : S →R continuously differentiable, then f is
concave if and only if
∀x, x0 ∈S :
f (x) −f (x0) ≤∇f (x0) · (x −x0)
(6)
strictly concave if and only if inequality (6) is strict for all x ̸= x0.
convex if and only if
∀x, x0 ∈S :
f (x) −f (x0) ≥∇f (x0) · (x −x0)
(7)
strictly convex if and only if inequality (7) is strict for all x ̸= x0.
ECON 2050 – Convexity
26 / 30
```

## PDF page 27

```text
By the theorem, the continuously differentiable function
f : R →R is concave if and only if for all x, x0 ∈R
f (x) −f (x0) ≤f ′(x0)(x −x0)
or
f (x) ≤f (x0) + f ′(x0)(x −x0).
Thus f is concave if and only if for every x0 ∈R, the graph of f lies below the tangent
line of f at point x0.
f : R2 →R is concave if and only if for all x, x0 ∈R2
f (x) ≤f (x0) + ∇f (x0)(x −x0).
Thus f is concave if and only if for every x0 ∈R2, the graph of f lies below the tangent
plane of f at point x0.
ECON 2050 – Convexity
27 / 30
```

## PDF page 28

```text
Geometric interpretation of concavity for functions of one or two variables:
ECON 2050 – Convexity
28 / 30
```

## PDF page 29

```text
Geometric interpretation of convexity for functions of one or two variables:
ECON 2050 – Convexity
29 / 30
```

## PDF page 30

```text
Example: Consider f : R2 →R, (x, y) ↦→x2 + y2.
f ’s tangent plane at point (x0, y0) is given by
g(x, y) = f (x0, y0) + ∇f (x0, y0) · (x −x0, y −y0)
= f (x0, y0) + ∂f (x0, y0)
∂x
(x −x0) + ∂f (x0, y0)
∂y
(y −y0)
= x2
0 + y2
0 + 2x0(x −x0) + 2y0(y −y0)
= 2x0x + 2y0y −x2
0 −y2
0
Thus we obtain
f (x, y) −g(x, y) = x2 + y2 −(2x0x + 2y0y −x2
0 −y2
0 ) = (x −x0)2 + (y −y0)2
As f (x, y) −g(x, y) > 0 for all (x, y) ̸= (x0, y0), we conclude by the previous theorem
that f is strictly convex.
ECON 2050 – Convexity
30 / 30
```
