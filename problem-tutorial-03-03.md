# Tutorial 3, Problem 3: A partial derivative from the definition

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-03-solutions.md) | [Original PDF](tutorial-03-solutions.pdf)

Topics: differentiation.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 3

[Original page](tutorial-03-solutions.pdf#page=3)

```text
Problem 3
Consider the function f : R2 →R, (x, y) 7→
xy
x2+y2+1. Determine ∂f(1,1)
∂x
directly
from the definition of the partial derivative, that is, by calculating the appropriate
limit.
Solution: We obtain
∂f(1, 1)
∂x
= lim
n→∞
f(1 + hn, 1) −f(1, 1)
hn
= lim
n→∞
1+hn
2+(1+hn)2 −1
3
hn
= lim
n→∞
3 + 3hn −2 −(1 + hn)2
3hn(2 + (1 + hn)2)
= lim
n→∞
hn(1 −hn)
3hn(2 + (1 + hn)2)
= lim
n→∞
(1 −hn)
3(2 + (1 + hn)2) = 1
9.
You are encouraged to check that if we derive the partial derivatives using the rules
of one-variable calculus by “holding other variables constant,” we get the same result.
```
