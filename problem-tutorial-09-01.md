# Tutorial 9, Problem 1: Graphical optimisation on different feasible sets

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-09-solutions.md) | [Original PDF](tutorial-09-solutions.pdf)

Topics: unconstrained; graphs.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-09-solutions.pdf#page=1)

```text
Problem 1
Let 𝑓∶ℝ2 →ℝbe given by 𝑓(𝑥, 𝑦) = 𝑥−𝑦. Solve the following problems graphically:
(a) max𝑥,𝑦∈ℝ𝑓(𝑥, 𝑦)
(b) max𝑥,𝑦∈ℝ𝑓(𝑥, 𝑦)
subject to 𝑥2 + 𝑦2 = 8
(c) max𝑥≥0, 𝑦≥0 𝑓(𝑥, 𝑦)
subject to 𝑥2 + 𝑦2 ≤8
Solution: In all three cases, the level curve of level 𝑐comprises all (𝑥, 𝑦) ∈ℝ2 that satisfy
𝑥−𝑦= 𝑐, or, equivalently, 𝑦= 𝑥−𝑐.
(a) We see that there is no maximum — “we can always increase 𝑐.” That is, the problem has
no solution.
2
-2
c=0
c=1
c=2
y
x
(b) We see that the solution is the tangency point depicted below.
2
-2
c=0
c=1
c=2
-4
4
c=4
(2,-2)
y
x
1
```

## PDF page 2

[Original page](tutorial-09-solutions.pdf#page=2)

```text
ECON 2050
S2 2026
By the implicit function theorem, the slope of the line tangent to the constraint set
{(𝑥, 𝑦) ∈ℝ2 ∶𝑥2 + 𝑦2 = 8} at (𝑥, 𝑦) is −2𝑥
2𝑦(as long as 𝑦≠0). Since the slope of
the level curves is 1, we must have −2𝑥
2𝑦= 1 at every point (𝑥, 𝑦) at which a level curve
is tangent to the constraint set. Hence 𝑥= −𝑦and 𝑥2 + 𝑦2 = 8 implies 2𝑥2 = 8 and
𝑥= ±2. The maximum is (2, −2) (at this point, the level curve of level 𝑐= 4 is tangent
to the constraint set.) At (−2, 2), 𝑓has a minimum in the constraint set.
(c) We see that the maximum is (√8, 0), a point on the level curve of level 𝑐= √8
2
-2
c=0
c=1
c=2
c=8
1/2
y
x
```
