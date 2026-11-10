# Tutorial 3, Problem 4: Production differential versus actual change

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-03-solutions.md) | [Original PDF](tutorial-03-solutions.pdf)

Topics: differentiation.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 3

[Original page](tutorial-03-solutions.pdf#page=3)

```text
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

## PDF page 4

[Original page](tutorial-03-solutions.pdf#page=4)

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
```
