# Tutorial 8 solutions: P3: Existence on a disk and a triangle; P4: Quadratic profit and a global maximum

PDF page 4 of 5.

[Page map](map-tutorial-08-solutions.md) | [Original PDF page](tutorial-08-solutions.pdf#page=4) | [Previous](page-tutorial-08-solutions-03.md) | [Next](page-tutorial-08-solutions-05.md)

Topics: convexity, existence, graphs, unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
(b) Observe that g = 4pr1 + 7pr2. Since the projections pr1 and pr2 are continuous, so
are 4pr1 and 7pr2 (in the future, you can just say that any affine, and therefore linear,
function is continuous). Then because the sum of continuous functions is continuous,
the objective function g is continuous.
The set D is closed because it contains all its boundary points (every point in the set
{(x, y) ∈R2 : x + 2y = 3, x = 0, y = 0} is a boundary point, which is contained in
D), and it is also bounded because for all (x, y) ∈D, ∥(x, y)∥≤3. Thus, D is compact.
Graphically, D is the triangle area in the picture below. The set of boundary points is
the lines in blue and red.
x
y
y = 0
x = 0
x + 2y = 3
O
1
2
3
0.5
1
1.5
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
