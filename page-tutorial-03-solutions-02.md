# Tutorial 3 solutions: P2: Domain, gradient, level curves and continuous differentiability

PDF page 2 of 5.

[Page map](map-tutorial-03-solutions.md) | [Original PDF page](tutorial-03-solutions.pdf#page=2) | [Previous](page-tutorial-03-solutions-01.md) | [Next](page-tutorial-03-solutions-03.md)

Topics: continuity, differentiation, graphs.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
(b) Recall that the gradient ∇f(x, y) of f at (x, y) is defined as ∇f(x, y) =

∂f(x,y)
∂x
, ∂f(x,y)
∂y

.
Calculate the gradient of f at every point (x, y).
Solution: We first determine f’s partial derivatives as
∂f(x, y)
∂x
= 1
ye
x
y +
2x
x2 + 1,
∂f(x, y)
∂y
= −x
y2e
x
y .
Then, the gradient of f at (x, y) is
∇f(x, y) =
1
ye
x
y +
2x
x2 + 1, −x
y2e
x
y

(c) Show that all points of the form (0, y), y ̸= 0, are located on the same level curve.
Solution: For every point (0, y) such that y ̸= 0
f(0, y) = e
0
y + ln(0 + 1) = e0 + ln(1) = 1 + 0 = 1.
Hence, f(0, y) does not depend on y, and all points of the form (0, y) are on the
level curve of level 1.
(d) (Harder) Determine, without checking the definition directly, whether f(x, y) is
continuously differentiable at the point (1, 1).
Solution: Recall a theorem in the lecture saying that if a function is continuously
partially differentiable, then it is (totally) differentiable. It now suffices to check
that both ∂f(x,y)
∂x
and ∂f(x,y)
∂y
are continuous at the point (1, 1). To show continuity,
we use the properties of continuous function described in the slides of Lecture 2.
Observe that both ∂f(x,y)
∂x
and ∂f(x,y)
∂y
are well-defined around (1, 1), and
∂f(x, y)
∂x
= 1
pr2
· e
pr1
pr2 +
2pr1
(pr1)2 + 1;
because ex, pr1, and pr2 are continuous, and the relevant operations (sum, prod-
uct, quotient, and composition) preserve continuity, we conclude that ∂f(x,y)
∂x
is
continuous at (1, 1). Similarly,
∂f(x, y)
∂y
= −pr1
(pr2)2 · e
pr1
pr2 ,
which is also continuous by an analogous argument.
2
```
