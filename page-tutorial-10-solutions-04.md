# Tutorial 10 solutions: P3: Log utility with a quadratic equality and multiplier interpretation

PDF page 4 of 7.

[Page map](map-tutorial-10-solutions.md) | [Original PDF page](tutorial-10-solutions.pdf#page=4) | [Previous](page-tutorial-10-solutions-03.md) | [Next](page-tutorial-10-solutions-05.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Solution:
(a) Letting g(x, y, z) = x2 + y2 + z then ∇g(x, y, z) = (2x, 2y, 1) ̸= (0, 0, 0). Therefore,
{∇g(x, y, z)} is linearly independent for every (x, y, z) in the constraint set. Thus, the
Lagrange conditions are necessary. The Lagrange conditions are
2
x −2λx = 0
⇔
x2 = 1
λ
5
y −2λy = 0
⇔
y2 = 5
2λ
1
z −λ = 0
⇔
z = 1
λ
x2 + y2 + z −32 = 0
Plugging the first three equations into the last gives
1 + 5
2 + 1 −32λ = 0
⇔
λ = 9
64;
plugging this back to the first three equations, we get that the unique point satisfying
the Lagrange condition is
(x∗, y∗, z∗, λ∗) =
 
8
3, 8
√
5
3
√
2, 64
9 , 9
64
!
.
(b) Let V (32) be the optimal value of the problem in part (a), and let V (32.1) be the optimal
value of the problem in this part. Using the multiplier λ∗corresponding to the solution
from part (a), and recall that λ∗can be interpreted as the per unit increase in objective
function value from the constraint for a sufficiently small amount:
V (32.1) ≈V (32)+0.1λ∗= 2(ln 8−ln 3)+5(ln 8+ln
√
5−ln 3−ln
√
2)+ln 64−ln 9+ 9
640
(The exact calculation doesn’t really matter; what matters is the first part.)
(c) The problem is equivalent to
max
(x,y)∈R2 −2 ln x −5 ln y −ln 3
s.t.
x2 + y2 = 29;
2 −x ≤0;
2 −y ≤0
The constraint set is visualized below; we see that it is compact. Because the objective
function is continuous, a solution exists.
4
```
