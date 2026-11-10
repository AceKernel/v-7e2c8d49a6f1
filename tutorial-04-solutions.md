# Tutorial 4 solutions: automatic text transcript

Original: [Tutorial 4 solutions PDF](tutorial-04-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
Econ 2050
Tutorial 4 Solution
Problem 1
Determine the (first-order) Taylor approximation of
f : R2
++ →R, (x, y) 7→ln(3x + 2y)
around the point a = (2, 1).
Solution: Since
∇f(x, y) =
∂f(x, y)
∂x
, ∂f(x, y)
∂y

=

3
3x + 2y,
2
3x + 2y

,
the first-order Taylor approximation around around the point a = (2, 1) equals
f(a) + ∇f(a) · (x −a) = ln(8) +
3
8, 2
8

· (x −2, y −1)
= ln(8) + 3
8(x −2) + 2
8(y −1)
= ln(8) + 3
8x + 2
8y −1
Problem 2
Suppose x(z) = z2 + 1, y(z) = ez, and
f(x, y) = 3x2
y .
Let F(z) ≡f(x(z), y(z)); calculate F ′(z) at z = 0.
Solution: We use the (generalized) chain rule to derive F ′(z):
F ′(z) = ∂f(x(z), y(z))
∂x
x′(z) + ∂f(x(z), y(z))
∂y
y′(z).
We have
∂f(x, y)
∂x
= 6x
y ,
and
∂f(x, y)
∂y
= −3x2
y2 .
1
```

## PDF page 2

```text
Econ 2050
Evaluating at x(z) = z2 + 1 and y(z) = ez:
∂f(x(z), y(z))
∂x
= 6(z2 + 1)
ez
,
and
∂f(x(z), y(z))
∂y
= −3(z2 + 1)2
e2z
.
Furthermore, x′(z) = 2z, and y′(z) = ez. Therefore,
F ′(z) = 12z(z2 + 1)
ez
−3(z2 + 1)2
ez
= 12z(z2 + 1) −3(z2 + 1)2
ez
.
Evaluating at z = 0 gets us
F ′(0) = 12(0)(02 + 1) −3(02 + 1)2
e0
= −3
1 = −3.
Problem 3
Suppose that it follows from the implicit function theorem that, in a neighborhood of
(x0, y0, z0), z is implicitly defined by the equation zex + ey −yez = 0 as a function of x and
y. Compute the partial derivatives ∂z
∂x and ∂z
∂y at the point (x0, y0).
Solution: The partial derivatives of f : R3 →R, (x, y, z) 7→zex +ey −yez at (x0, y0, z0) are:
∂f(x0, y0, z0)
∂x
= z0ex0
∂f(x0, y0, z0)
∂y
= ey0 −ez0
∂f(x0, y0, z0)
∂z
= ex0 −y0ez0
We must have ∂f(x0, y0, z0)
∂z
̸= 0, otherwise, the implicit function theorem would not apply.
Using the implicit function theorem, we obtain:
∂z(x0, y0)
∂x
= −
∂f(x0,y0,z0)
∂x
∂f(x0,y0,z0)
∂z
= −
z0ex0
ex0 −y0ez0
∂z(x0, y0)
∂y
= −
∂f(x0,y0,z0)
∂y
∂f(x0,y0,z0)
∂z
= −ey0 −ez0
ex0 −y0ez0 =
ez0 −ey0
ex0 −y0ez0
Problem 4
Obtain an equation of the tangent line to the level curve of f : R2 →R at the point
1. (x0, y0) = (1, 1) if f(x, y) = xexy
2. (x0, y0) = (−1, 2) if f(x, y) = y −x2
2
```

## PDF page 3

```text
Econ 2050
3. (Extra Practice Problem) (x0, y0) = (1, 2) if f(x, y) = yx
Solution:
1. Since f(1, 1) = e, the level curve of f through (x0, y0) = (1, 1) is L = {(x, y) ∈R2 :
xexy = e}. From
∂f(x, y)
∂x
= exy + xyexy = exy(1 + xy)
∂f(x, y)
∂y
= x2exy
we can conclude that f is continuously differentiable (as both its partial derivatives
are continuous), and that ∂f(1,1)
∂y
= e ̸= 0. Hence by the implicit function theorem, a
continuously differentiable function y = g(x) whose graph describes L in a vicinity
of (1, 1) exists, and
g′(1) = −
∂f(1,1)
∂x
∂f(1,1)
∂y
= −e1·1(1 + 1 · 1)
12e1·1
= −2
Therefore, the equation of the tangent line g to the level curve L at (1, 1) is
h(x) = y0 + g′(x0)(x −x0) = 1 −2(x −1) = −2x + 3
2. Similarly, in this case, from
∂f(x, y)
∂x
= −2x
∂f(x, y)
∂y
= 1
it follows that f is continuously differentiable, and that ∂f(−1,2)
∂y
= 1 ̸= 0. Hence by
the implicit function theorem, a continuously differentiable function y = g(x) whose
graph describes L in a vicinity of (−1, 2) exists, and
g′(−1) = −
∂f(−1,2)
∂x
∂f(−1,2)
∂y
= −2
Therefore, the equation of the tangent line h to the level curve L at (−1, 2) is
h(x) = y0 + g′(x0)(x −x0) = 2 + (−2)(x −(−1)) = −2x
3. Finally, in this case, from
∂f(x, y)
∂x
= y
∂f(x, y)
∂y
= x
3
```

## PDF page 4

```text
Econ 2050
it follows that f is continuously differentiable, and that ∂f(1,2)
∂y
= 1 ̸= 0. Hence by
the implicit function theorem, a continuously differentiable function y = g(x) whose
graph describes L in a vicinity of (1, 2) exists, and
g′(1) = −
∂f(1,2)
∂x
∂f(1,2)
∂y
= −2
Therefore, the equation of the tangent line h to the level curve L at (1, 2) is
h(x) = y0 + g′(x0)(x −x0) = 2 + (−2)(x −1) = −2x + 4
Problem 5
Calculate the Hessian matrix of each of the following functions.
(a) f : R2 →R, (x, y) 7→xexy
Solution: (Sketch only) We obtain
∇f(x, y) =
exy + xyexy,
x2exy
H(x, y) = exy

2y + xy2
2x + x2y
2x + x2y
x3

(b) f : R2
++ →R, (x, y) 7→ln(xy + y2 + x2)
Solution: (Sketch only) We obtain
∇f(x, y) =

y + 2x
xy + y2 + x2,
x + 2y
xy + y2 + x2

H(x, y) =
1
(xy + y2 + x2)2

y2 −2xy −2x2
−x2 −y2 −4xy
−x2 −y2 −4xy
x2 −2y2 −2xy

(c) (Harder; Extra Practice Problem) f : {(x, y) ∈R2
+ : xy ≤3} →R, (x, y) 7→
p
3x −x2y
Solution: (Sketch only) We obtain
∇f(x, y) =
 
3 −2xy
2
p
3x −x2y
,
−x2
2
p
3x −x2y
!
H(x, y) =
1
4 (3x −x2y)
3
2

−9
−9x2 + 2x3y
−9x2 + 2x3y
−x4

4
```

## PDF page 5

```text
Econ 2050
Problem 6 (Extra Practice Problem)
Suppose that it follows from the implicit function theorem that, in a neighborhood of
(x0, y0, z0), z is implicitly defined by the equation x2 + y2 + z2 = a2 as a function of x and
y. Compute the total derivative Dz(x0, y0).
Solution: If we let f : R3 →R, (x, y, z) 7→x2 + y2 + z2 −a2 then the equation above is
equivalent to f(x, y, z) = 0. We have
∂f(x, y, z)
∂x
= 2x
∂f(x, y, z)
∂y
= 2y
∂f(x, y, z)
∂z
= 2z
(Since all partial derivatives of f are continuous, f is continuously differentiable.) Since the
implicit function theorem applied, ∂f(x0,y0,z0)
∂z
= 2z0 ̸= 0. By the implicit function theorem,
∂z(x0, y0)
∂x
= −
∂f(x0,y0,z0)
∂x
∂f(x0,y0,z0)
∂z
= −2x0
2z0
= −x0
z0
∂z(x0, y0)
∂y
= −
∂f(x0,y0,z0)
∂y
∂f(x0,y0,z0)
∂z
= −2y0
2z0
= −y0
z0
Therefore, Dz(x0, y0) = ∇z(x0, y0) =

−x0
z0
, −y0
z0

.
(Alternatively, from Df(x0, y0, z0) · (dx, dy, dz) = 0 we obtain
(2x0, 2y0, 2z0) · (dx, dy, dz) = 2x0dx + 2y0dy + 2z0dz = 0
or
dz = −2x0
2z0
dx −2y0
2z0
dy = −x0
z0
dx −y0
z0
dy,
and we can see that Dz(x0, y0) =

−x0
z0
, −y0
z0

.)
5
```
