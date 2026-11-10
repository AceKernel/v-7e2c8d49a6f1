# Tutorial 3, Problem 1: Partial derivatives and evaluation

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-03-solutions.md) | [Original PDF](tutorial-03-solutions.pdf)

Topics: differentiation.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-03-solutions.pdf#page=1)

```text
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
```
