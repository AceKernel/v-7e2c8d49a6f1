# Tutorial 4 solutions: P4: Tangent lines to implicit level curves; P5: Hessian calculations

PDF page 4 of 5.

[Page map](map-tutorial-04-solutions.md) | [Original PDF page](tutorial-04-solutions.pdf#page=4) | [Previous](page-tutorial-04-solutions-03.md) | [Next](page-tutorial-04-solutions-05.md)

Topics: chain-hessian, graphs, implicit.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
