# Tutorial 3 solutions: P4: Production differential versus actual change; P5: Chain rule for logarithmic and square-root functions

PDF page 4 of 5.

[Page map](map-tutorial-03-solutions.md) | [Original PDF page](tutorial-03-solutions.pdf#page=4) | [Previous](page-tutorial-03-solutions-03.md) | [Next](page-tutorial-03-solutions-05.md)

Topics: chain-hessian, differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
and
f(10000, 625) = 4(10000)3/4(625)1/4 = 4 · 1000 · 5 = 20000
we obtain
∂f(10000, 625)
∂K
= 3
4
20000
10000 = 3
2,
∂f(10000, 625)
∂L
= 1
4
20000
625
= 8,
and can conclude that the production of output increases by
∆f ≈df = 3
2 · dK + 8 · dL = 9.5
units.
Alternatively, we can compute the value of the production function for the old
and the new values of K and L and compute the difference. Currently, the firm
employs K = 10000 units of capital, L = 625 units of labor, and, as we saw above,
produces f(10000, 625) = 20000 units of output. With the increased amounts of
capital and labor, the firm would produce
f(10001, 626) = 4(10001)3/4(626)1/4 ≈20009.4958
units of output. Hence, increasing the input of both capital and labor by 1 unit each
increases output by approximately 9.4958 units.
(Just looking at this particular question, it may seem that the second approach
is actually easier, and that our efforts to understand derivatives are not paying off.
However, soon, when we discuss how to optimize [= maximize or minimize] func-
tions, this changes dramatically. For optimization problems, approaches using deriva-
tives will be “easy,” while those relying on just computing different values for f will
be cumbersome or even not viable.)
Problem 5 (Extra Practice Problem)
For each of the following functions f, calculate the partial derivatives, and eval-
uate them at the point (1, 1).
(a) f : R2 →R, (x, y) 7→ln(x2 + y2 + 1)
(b) f : R2
++ →R, (x, y) 7→
p
xy + y3
Solution:
(a) To find ∂f(x,y)
∂x
, we treat y as a constant, and use the chain rule:
1. Take the derivative of the outer function, ln(u), where u ≡x2 +y2 +1, which
is 1
u.
4
```
