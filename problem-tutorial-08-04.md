# Tutorial 8, Problem 4: Quadratic profit and a global maximum

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-08-solutions.md) | [Original PDF](tutorial-08-solutions.pdf)

Topics: unconstrained; convexity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 4

[Original page](tutorial-08-solutions.pdf#page=4)

```text
Problem 4 (Extra Practice Problem)
An artisan uses xh units of labor and xm units of a unique material to produce a product.
Her profits if employing (xh, xm) ≥0 units of the mentioned factors are
π(xh, xm) = 20xh + 26xm + 4xhxm −4x2
h −3x2
m
Find the values of xh and xm that maximize the artisan’s profits.
Solution: To find the global maxima of π, first show that the objective function π is concave.
To that end, observe that if the term 4xhxm is absent, then π(xh, xm) can be written as the
sum of two functions, one is a function of xh only, and the other is a function of xm only,
and both functions are concave. If this is the case, π must also be concave by the result in
Tutorial 7 Problem 2. Therefore, we aim to “eliminate” the term 4xhxm by completing the
square.
Note that −4x2
h + 4xhxm −x2
m = −(2xh −xm)2, and therefore
π(xh, xm) = 20xh + 26xm −2x2
m −(2xh −xm)2.
Let π1(xh, xm) ≡20xh + 26xm −2x2
m; by the result in Tutorial 7 Problem 2, it is a concave
function. Also let π2(xh, xm) ≡−(2xh −xm)2; by the result in Problem 1, π2 is also a
concave function. Then since π = π1 + π2, and the sum of concave functions is a concave
function, π is also concave.
From
∂π(xh, xm)
∂xh
= 20 + 4xm −8xh = 0
⇐⇒
5 + xm = 2xh
∂π(xh, xm)
∂xm
= 26 + 4xh −6xm = 0
⇐⇒
3xm −13 = 2xh
4
```

## PDF page 5

[Original page](tutorial-08-solutions.pdf#page=5)

```text
ECON 2050
S2 2026
we see that the unique critical point of π is (x∗
h, x∗
m) = (7, 9). Since π is concave, the unique
critical point (x∗
h, x∗
m) = (7, 9) must be a global maximum.
Summarizing, choosing xh = 7 and xm = 9 maximizes the artisan’s profits.
5
```
