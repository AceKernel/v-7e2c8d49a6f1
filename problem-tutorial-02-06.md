# Tutorial 2, Problem 6: Failure of continuous extension

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-02-solutions.md) | [Original PDF](tutorial-02-solutions.pdf)

Topics: continuity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 4

[Original page](tutorial-02-solutions.pdf#page=4)

```text
Problem 6 (Extra Practice Problem)
Let A ⊊Rk. We say that a function f : Rk\A →R can be continuously
extended (to Rk) if there is a continuous function g : Rk →R such that f(x) =
g(x) for all x ∈Rk\A. Prove that the following functions cannot be continuously
extended.1
(In the lectures, even though we did not use this language, we showed that f :
R2\{(0, 0)} →R, (x, y) 7→
xy
x2+y2 cannot be continuously extended.)
(a) f : R2\{(0, 0)} →R, (x, y) 7→
xy2
x4+y4
(Hint: Consider a sequence in the x-y-plane that approaches (0, 0) along the
diagonal.)
1Part (a) is similar to SB, Exercise 13.21. Note that in SB, there is a typo: SB erroneously write x2 instead of
x4 in the function - this is Part (b), and requires a different hint than the one given in SB!
4
```

## PDF page 5

[Original page](tutorial-02-solutions.pdf#page=5)

```text
(b) f : R2\{(0, 0)} →R, (x, y) 7→
xy2
x2+y4
(Hint: Consider a sequence in the x-y-plane that approaches (0, 0) along a line,
and a sequence that approaches (0, 0) along a certain parabola.)
Solution:
(a) Consider the sequence
 1
n, 1
n

n∈N. Since 1
n →0, this sequence converges to (0, 0),
and if g was a continuous extension of f, then we would have f
 1
n, 1
n

→g(0, 0).
However,
f
1
n, 1
n

=
1
n
 1
n
2
 1
n
4 +
 1
n
4 = n
2,
implying that
f
 1
n, 1
n

n∈N diverges. Therefore, it is impossible to extend f
continuously.
(b) Consider the sequences
 1
n, 0

n∈N and
 1
n2, 1
n

n∈N. Both of these sequences con-
verge to (0, 0) (the second sequence along the parabola x = y2). However,
f
1
n, 0

= 0 →0
and
f
 1
n2, 1
n

=
1
n2
 1
n
2
 1
n2
2 +
 1
n
4 = 1
2 →1
2,
implying that no extension of f can be continuous.
This is a particularly striking example of how difficult it can be to prove that a
function is continuous: at first, it may seem as if letting f(0, 0) = 0 continuously
extends f. This is because for all sequences (xn)n∈N in R2 that approach (0, 0)
on a line, we get f(xn) →0. (To see this, note that for y = mx, m ∈R, we
have f(x, y) =
x(mx)2
x2+(mx)4 =
m2x
1+m4x2. If x →0, we get f(x, mx) →
0
1+0 = 0.
The only line that is not of the form y = mx is x = 0. In this case, f(0, y) = 0
for y ̸= 0 and so if y approaches 0, f(0, y) →0.) However, continuity at (0, 0)
requires that f(xn) →0 for all (xn)n∈N converging to (0, 0), even those who do
not approach (0, 0) on a line!
```
