# Tutorial 9 solutions: P3: A linear program and sensitivity; P4: Duals with free variables and equalities; P5: Factory operating-cost minimisation and its dual

PDF page 5 of 6.

[Page map](map-tutorial-09-solutions.md) | [Original PDF page](tutorial-09-solutions.pdf#page=5) | [Previous](page-tutorial-09-solutions-04.md) | [Next](page-tutorial-09-solutions-06.md)

Topics: duality, linear-programming.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Problem 4
Write down the dual of the following linear programming problems.
(a)
max
𝑥1 + 𝑥2 −3𝑥3
s.t.
𝑥1 + 2𝑥2 −3𝑥3
≤4
4𝑥1 + 5𝑥2 −9𝑥3
≤13
(b)
max
𝑥1 + 𝑥2 −3𝑥3
s.t.
𝑥1 + 2𝑥2 −3𝑥3
= 4
4𝑥1 + 5𝑥2 −9𝑥3
= 13
Solution: Letting
c = (1
1
−3) ,
A = (
1
2
−3
4
5
−9) ,
and
b = (
4
13) ,
the linear programs in parts (a) and (b) can be written as
max c ⋅x
s.t. Ax ≤b
and
max c ⋅x
s.t. Ax = b,
respectively. Now using the observations in lecture 9 slides under the “writing down the
dual” section, their duals are
min y ⋅b
s.t. yA = c, y ≥0,
and
min y ⋅b
s.t. yA = c,
respectively. Therefore, the dual of the problem in part (a) is
min
4𝑦1 + 13𝑦2
s.t.
𝑦1 + 4𝑦2 = 1
2𝑦1 + 5𝑦2 = 1
−3𝑦1 −9𝑦2 = −3
𝑦1 ≥0, 𝑦2 ≥0
and the dual of the problem in part (b) is
min
4𝑦1 + 13𝑦2
s.t.
𝑦1 + 4𝑦2 = 1
2𝑦1 + 5𝑦2 = 1
−3𝑦1 −9𝑦2 = −3
Problem 5 (Extra Practice Problem)
5
```
