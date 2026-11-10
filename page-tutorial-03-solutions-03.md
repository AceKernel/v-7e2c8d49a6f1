# Tutorial 3 solutions: P3: A partial derivative from the definition; P4: Production differential versus actual change

PDF page 3 of 5.

[Page map](map-tutorial-03-solutions.md) | [Original PDF page](tutorial-03-solutions.pdf#page=3) | [Previous](page-tutorial-03-solutions-02.md) | [Next](page-tutorial-03-solutions-04.md)

Topics: differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
Problem 4
The production function of a firm is f : R2
+ →R, (K, L) 7→4K
3
4L
1
4. Currently,
the firm is using 10,000 units of capital (K) and employing 625 workers (L). The CEO
of the firm would like to know how the production of output (f(L, K)) changes when
the capital is increased by one unit and one more worker is employed. Can you help
her?
Solution: In order to compute the change in the output production level, we can use
derivatives (keep in mind that this approach provides an approximation of the exact
answer). If capital changes by dK = 1 and labor by dL = 1, then the output will
change by
∆f ≈df = ∂f(10000, 625)
∂K
· dK + ∂f(10000, 625)
∂L
· dL.
From
∂f(K, L)
∂K
= 43
4K−1/4L1/4 = 3
4
4K3/4L1/4
K
= 3
4
f(K, L)
K
,
∂f(K, L)
∂L
= 41
4K3/4L−3/4 = 1
4
4K3/4L1/4
L
= 1
4
f(K, L)
L
,
3
```
