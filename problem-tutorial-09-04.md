# Tutorial 9, Problem 4: Duals with free variables and equalities

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-09-solutions.md) | [Original PDF](tutorial-09-solutions.pdf)

Topics: duality.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 5

[Original page](tutorial-09-solutions.pdf#page=5)

```text
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
```
