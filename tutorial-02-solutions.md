# Tutorial 2 solutions: automatic text transcript

Original: [Tutorial 2 solutions PDF](tutorial-02-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
Econ 2050
Tutorial 2
Problem 1
Let f denote an arbitrary function f : R2 →R. For each of the following state-
ments, determine whether the statement is true or false. If false, provide an explana-
tion or a counterexample.
(a) If f(x0, y0) = f(x1, y1), then x0 = x1 and y0 = y1.
Solution: False. Counterexample: If we let (x0, y0) = (1, 2), (x1, y1) = (−1, −2)
and f : R2 →R, (x, y) 7→xy, then f(1, 2) = 2 = f(−1, −2), but x0 = 1 ̸=
−1 = x1 and y0 = 2 ̸= −2 = y1.
(b) If a ∈R then f(ax, ay) = a2f(x, y).
Solution: False. Counterexample: For f : R2 →R, (x, y) 7→x+y and any a ∈R,
we have f(ax, ay) = ax + ay = a(x + y) = af(x, y). And if a /∈{0, 1} and
f(x, y) ̸= 0 (which is e.g. the case if x = y ̸= 0), then af(x, y) ̸= a2f(x, y).
(c) A vertical line (that is, a line parallel to the “z-axis”) can cross the graph of f at
most once.
Solution: True. By definition of a function, f maps each (x, y) to a unique real
number z.
(d) Two level curves of f can intersect.
Solution: False. If this statement was true, then there would exist a point (x, y)
that would be on two distinct level curves, say on the level curves of level C1
and of level C2(̸= C1). That is, we would have f(x, y) = C1 and f(x, y) = C2.
Contradiction, since C1 ̸= C2.
Problem 2
Recall that a level curve of a function (of two variables) f is a subset of f’s do-
main whose elements are the points (x, y) for which for some k ∈R, f(x, y) = k.
Determine the domain on which the following functions can be defined and draw a
few level curves for each of them.
(a) f(x, y) = (x −1)2 + (y + 2)2
(b) f(x, y) = x + y2 + 1
1
```

## PDF page 2

```text
Solution: These three functions can be defined for all (x, y) ∈R2.
(a) f(x, y) = (x −1)2 + (y + 2)2
(b) f(x, y) = x + y2 + 1
One level curve we determine here is for k = 1. Notice that f(x, y) = 1 is
equivalent to x + y2 + 1 = 1, which yields x = −y2. This level curve has the
same shape as those in the figure below and contains (x, y) = (0, 0) so it goes
through the origin.
Problem 3
Recall that ln(·), sin(·), and cos(·) are continuous. Prove that the following func-
tions are continuous.
(a) f : R →R, x 7→(cos x)2
(b) f : R2 →R2, (x, y) 7→(ln(x4 + 1), ln(y4 + 1))
(c) f : R2 →R, (x, y) 7→sin(x2) + sin(y2)
Solution: (Sketch only)
(a) f = g ◦cos for g : R →R, x 7→x2
(b) Each component function fi : R2 →R, (x1, x2) 7→ln(x4
i + 1) of f = (f1, f2) is
continuous, as fi = ln ◦g ◦pri for g : R →R, x 7→x4 + 1
2
```

## PDF page 3

```text
(c) f = sin ◦g ◦pr1 + sin ◦g ◦pr2 for g : R →R, x 7→x2
Problem 4
The level curves of a production function Q(K, L) are called isoquants. Obtain
and plot a few isoquants for the following production functions.
(a) Q(K, L) = K
1
2L
1
2
(b) Q(K, L) = 0.5 ln(K) + 0.5 ln(L)
Solution:
(a) Q(K, L) = K
1
2L
1
2
The level curve of level C is characterized by the equation K
1
2L
1
2 = C, or, equiv-
alently,
(K
1
2L
1
2)2 = C2,
KL = C2,
L = C2
K
(b) Q(K, L) = 0.5 ln(K) + 0.5 ln(L)
The level curve of level C is characterized by the equation 0.5 ln(K)+0.5 ln(L) =
C, or, equivalently,
eln(K
1
2 )+ln(L
1
2 ) = eC,
eln(K
1
2 )eln(L
1
2 ) = eC,
K
1
2L
1
2 = eC,
from which it follows that the contour plot of this production function is identical
to that in the figure for part (a).
3
```

## PDF page 4

```text
Problem 5
(a) Write down the formula for a linear function g with domain R2 and codomain R
that has the property that g(7, 2) −g(3, 2) = 8 and g(7, 5) −g(3, 2) = 5.
Solution: Since g is linear, we know there exists a = (a1, a2) such that g(x) =
a · x = a1x1 + a2x2 for all x ∈R2. From
g(7, 2) −g(3, 2) = a1 · 7 + a2 · 2 −(a1 · 3 + a2 · 2) = 4a1 = 8
we conclude that a1 = 2. From
g(7, 5) −g(3, 2) = a1 · 7 + a2 · 5 −(a1 · 3 + a2 · 2) = 4a1 + 3a2 = 8 + 3a2 = 5
we conclude that a2 = −1. Hence g : R2 →R, x 7→(2, −1) · x.
(b) Consider ˆg : R2 →R, x 7→g(x) + 2, where g is the linear function from (a).
How does the value of ˆg change if x changes
(i) from (−3, 0) to (2, 1)?
(ii) from (2, 5) to (1, 3)?
Solution: The change dy in the value of ˆg if its variables change by dx is given by
dy = (2, −1) · dx.
(i) Here, dx = (2, 1) −(−3, 0) = (5, 1) and thus dy = (2, −1) · (5, 1) =
10 −1 = 9.
(ii) Here, dx = (1, 3) −(2, 5) = (−1, −2) and thus dy = (2, −1) · (−1, −2) =
−2 + 2 = 0.
Problem 6 (Extra Practice Problem)
Let A ⊊Rk. We say that a function f : Rk\A →R can be continuously
extended (to Rk) if there is a continuous function g : Rk →R such that f(x) =
g(x) for all x ∈Rk\A. Prove that the following functions cannot be continuously
extended.1
(In the lectures, even though we did not use this language, we showed that f :
R2\{(0, 0)} →R, (x, y) 7→
xy
x2+y2 cannot be continuously extended.)
(a) f : R2\{(0, 0)} →R, (x, y) 7→
xy2
x4+y4
(Hint: Consider a sequence in the x-y-plane that approaches (0, 0) along the
diagonal.)
1Part (a) is similar to SB, Exercise 13.21. Note that in SB, there is a typo: SB erroneously write x2 instead of
x4 in the function - this is Part (b), and requires a different hint than the one given in SB!
4
```

## PDF page 5

```text
(b) f : R2\{(0, 0)} →R, (x, y) 7→
xy2
x2+y4
(Hint: Consider a sequence in the x-y-plane that approaches (0, 0) along a line,
and a sequence that approaches (0, 0) along a certain parabola.)
Solution:
(a) Consider the sequence
 1
n, 1
n

n∈N. Since 1
n →0, this sequence converges to (0, 0),
and if g was a continuous extension of f, then we would have f
 1
n, 1
n

→g(0, 0).
However,
f
1
n, 1
n

=
1
n
 1
n
2
 1
n
4 +
 1
n
4 = n
2,
implying that
f
 1
n, 1
n

n∈N diverges. Therefore, it is impossible to extend f
continuously.
(b) Consider the sequences
 1
n, 0

n∈N and
 1
n2, 1
n

n∈N. Both of these sequences con-
verge to (0, 0) (the second sequence along the parabola x = y2). However,
f
1
n, 0

= 0 →0
and
f
 1
n2, 1
n

=
1
n2
 1
n
2
 1
n2
2 +
 1
n
4 = 1
2 →1
2,
implying that no extension of f can be continuous.
This is a particularly striking example of how difficult it can be to prove that a
function is continuous: at first, it may seem as if letting f(0, 0) = 0 continuously
extends f. This is because for all sequences (xn)n∈N in R2 that approach (0, 0)
on a line, we get f(xn) →0. (To see this, note that for y = mx, m ∈R, we
have f(x, y) =
x(mx)2
x2+(mx)4 =
m2x
1+m4x2. If x →0, we get f(x, mx) →
0
1+0 = 0.
The only line that is not of the form y = mx is x = 0. In this case, f(0, y) = 0
for y ̸= 0 and so if y approaches 0, f(0, y) →0.) However, continuity at (0, 0)
requires that f(xn) →0 for all (xn)n∈N converging to (0, 0), even those who do
not approach (0, 0) on a line!
Problem 7 (Extra Practice Problem)
Determine whether the function f : R2\{(x1, x2) ∈R2 : x1 = x2} →R, (x1, x2) 7→
x2
1−x2
2
x1−x2 can be continuously extended to R2. If yes, show how. If no, prove why.
Solution: Yes, f can be continuously extended. Clearly,
g : R2 →R, (x1, x2) 7→
(
x2
1−x2
2
x1−x2
if x1 ̸= x2
x1 + x2
if x1 = x2
5
```

## PDF page 6

```text
extends f to R2. Note that
x2
1 −x2
2
x1 −x2
= (x1 + x2)(x1 −x2)
x1 −x2
= x1 + x2,
and that therefore, we can simplify and write g as g : R2 →R, (x1, x2) 7→x1 + x2.
Since g = pr1 + pr2, g is continuous. To sum up, g continuously extends f.
6
```
