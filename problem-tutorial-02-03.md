# Tutorial 2, Problem 3: Continuity through projections and composition

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-02-solutions.md) | [Original PDF](tutorial-02-solutions.pdf)

Topics: continuity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 2

[Original page](tutorial-02-solutions.pdf#page=2)

```text
Problem 3
Recall that ln(·), sin(·), and cos(·) are continuous. Prove that the following func-
tions are continuous.
(a) f : R →R, x 7→(cos x)2
(b) f : R2 →R2, (x, y) 7→(ln(x4 + 1), ln(y4 + 1))
(c) f : R2 →R, (x, y) 7→sin(x2) + sin(y2)
Solution: (Sketch only)
(a) f = g ◦cos for g : R →R, x 7→x2
(b) Each component function fi : R2 →R, (x1, x2) 7→ln(x4
i + 1) of f = (f1, f2) is
continuous, as fi = ln ◦g ◦pri for g : R →R, x 7→x4 + 1
2
```

## PDF page 3

[Original page](tutorial-02-solutions.pdf#page=3)

```text
(c) f = sin ◦g ◦pr1 + sin ◦g ◦pr2 for g : R →R, x 7→x2
```
