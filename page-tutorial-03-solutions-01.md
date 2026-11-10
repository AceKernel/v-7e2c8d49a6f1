# Tutorial 3 solutions: P1: Partial derivatives and evaluation; P2: Domain, gradient, level curves and continuous differentiability

PDF page 1 of 5.

[Page map](map-tutorial-03-solutions.md) | [Original PDF page](tutorial-03-solutions.pdf#page=1) | [Next](page-tutorial-03-solutions-02.md)

Topics: continuity, differentiation, graphs.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON2050
S2 2026
Tutorial 3 Solution
Problem 1
(a) Let
f : R3
++ →R, (x1, x2, x3) 7→3x2
1 + ex2
2x3
.
Compute all partial derivatives.
(b) Evaluate the partial derivative of f with respect to x3 at the point (1, 2, 3).
Solution:
(a) The partial derivatives are
∂f(x1, x2, x3)
∂x1
= 3x1
x3
∂f(x1, x2, x3)
∂x2
= ex2
2x3
∂f(x1, x2, x3)
∂x3
= −3x2
1 −ex2
2x2
3
To derive them, simply hold all other variables constant. This allows you to treat
the function as a function of one variable—the one you are differentiating with
respect to—and apply the rules of differentiation for functions of one variables at
the beginning of Lecture 3 slides.
(b) We obtain
∂f(1, 2, 3)
∂x3
= −3 · 12 −e2
2 · 32
= −3 −e2
18
.
Problem 2
You are given the function f : D →R, (x, y) 7→e
x
y + ln(x2 + 1), where D is the
largest subset of R2 on which f is well-defined.
(a) Determine D.
Solution: The domain of f is D = {(x, y) ∈R2 : y ̸= 0}: if y = 0, e
x
y is not
well-defined.
1
```
