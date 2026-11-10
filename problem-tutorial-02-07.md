# Tutorial 2, Problem 7: Continuous extension across a diagonal

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-02-solutions.md) | [Original PDF](tutorial-02-solutions.pdf)

Topics: continuity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 5

[Original page](tutorial-02-solutions.pdf#page=5)

```text
Problem 7 (Extra Practice Problem)
Determine whether the function f : R2\{(x1, x2) ∈R2 : x1 = x2} →R, (x1, x2) 7→
x2
1−x2
2
x1−x2 can be continuously extended to R2. If yes, show how. If no, prove why.
Solution: Yes, f can be continuously extended. Clearly,
g : R2 →R, (x1, x2) 7→
(
x2
1−x2
2
x1−x2
if x1 ̸= x2
x1 + x2
if x1 = x2
5
```

## PDF page 6

[Original page](tutorial-02-solutions.pdf#page=6)

```text
extends f to R2. Note that
x2
1 −x2
2
x1 −x2
= (x1 + x2)(x1 −x2)
x1 −x2
= x1 + x2,
and that therefore, we can simplify and write g as g : R2 →R, (x1, x2) 7→x1 + x2.
Since g = pr1 + pr2, g is continuous. To sum up, g continuously extends f.
6
```
