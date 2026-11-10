# Tutorial 11 solutions: P1: Nonnegative KKT with linear constraints

PDF page 1 of 4.

[Page map](map-tutorial-11-solutions.md) | [Original PDF page](tutorial-11-solutions.pdf#page=1) | [Next](page-tutorial-11-solutions-02.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Tutorial 11 Solution
Problem 1
Consider the following nonlinear programming problem
max 2x −2y2
s.t.
2x −y ≤5, y ≤4, x ≥0, y ≥0.
(a) Try to solve (at least roughly) the problem graphically.
(b) Solve the problem using the KKT approach.
Solution:
(a) The level curve of the objective function of level C is defined by the equation x = y2+ 1
2C.
You have to draw quite precisely to see the exact solution: it is (x∗, y∗) = (21/8, 1/4).
C
y = −5 + 2x
y = 4
2x −2y2 = 5.125
x
y
−1
0
1
2
3
4
5
−1
0
1
2
3
4
5
(b) Because the constraint functions are all affine, the KKT conditions are necessary.
The KKT conditions are
2 −2λ1 ≤0,
x ≥0,
x(2 −2λ1) = 0
−4y + λ1 −λ2 ≤0,
y ≥0,
y(−4y + λ1 −λ2) = 0
2x −y −5 ≤0,
λ1 ≥0,
λ1(2x −y −5) = 0
y −4 ≤0,
λ2 ≥0,
λ2(y −4) = 0
We see that
• x > 0 and λ1 = 1: Because 2 −2λ1 ≤0, we must have λ1 > 0. Hence by
complementary slackness [λ1(2x −y −5) = 0], 2x −y = 5. But this implies that
x = 0: if x = 0, 2(0) −y = 5 and thus y = −5 < 0, a contradiction. Hence x > 0;
by complementary slackness [x(2 −2λ1) = 0], we have λ1 = 1.
1
```
