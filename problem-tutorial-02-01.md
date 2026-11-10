# Tutorial 2, Problem 1: Function statements and counterexamples

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-02-solutions.md) | [Original PDF](tutorial-02-solutions.pdf)

Topics: notation; continuity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-02-solutions.pdf#page=1)

```text
Problem 1
Let f denote an arbitrary function f : R2 →R. For each of the following state-
ments, determine whether the statement is true or false. If false, provide an explana-
tion or a counterexample.
(a) If f(x0, y0) = f(x1, y1), then x0 = x1 and y0 = y1.
Solution: False. Counterexample: If we let (x0, y0) = (1, 2), (x1, y1) = (−1, −2)
and f : R2 →R, (x, y) 7→xy, then f(1, 2) = 2 = f(−1, −2), but x0 = 1 ̸=
−1 = x1 and y0 = 2 ̸= −2 = y1.
(b) If a ∈R then f(ax, ay) = a2f(x, y).
Solution: False. Counterexample: For f : R2 →R, (x, y) 7→x+y and any a ∈R,
we have f(ax, ay) = ax + ay = a(x + y) = af(x, y). And if a /∈{0, 1} and
f(x, y) ̸= 0 (which is e.g. the case if x = y ̸= 0), then af(x, y) ̸= a2f(x, y).
(c) A vertical line (that is, a line parallel to the “z-axis”) can cross the graph of f at
most once.
Solution: True. By definition of a function, f maps each (x, y) to a unique real
number z.
(d) Two level curves of f can intersect.
Solution: False. If this statement was true, then there would exist a point (x, y)
that would be on two distinct level curves, say on the level curves of level C1
and of level C2(̸= C1). That is, we would have f(x, y) = C1 and f(x, y) = C2.
Contradiction, since C1 ̸= C2.
```
