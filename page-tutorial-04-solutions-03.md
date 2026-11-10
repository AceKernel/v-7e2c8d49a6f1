# Tutorial 4 solutions: P4: Tangent lines to implicit level curves

PDF page 3 of 5.

[Page map](map-tutorial-04-solutions.md) | [Original PDF page](tutorial-04-solutions.pdf#page=3) | [Previous](page-tutorial-04-solutions-02.md) | [Next](page-tutorial-04-solutions-04.md)

Topics: graphs, implicit.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
