# Tutorial 2 solutions: P5: Linear and affine functions; P6: Failure of continuous extension

PDF page 4 of 6.

[Page map](map-tutorial-02-solutions.md) | [Original PDF page](tutorial-02-solutions.pdf#page=4) | [Previous](page-tutorial-02-solutions-03.md) | [Next](page-tutorial-02-solutions-05.md)

Topics: continuity, differentiation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Problem 5
(a) Write down the formula for a linear function g with domain R2 and codomain R
that has the property that g(7, 2) −g(3, 2) = 8 and g(7, 5) −g(3, 2) = 5.
Solution: Since g is linear, we know there exists a = (a1, a2) such that g(x) =
a · x = a1x1 + a2x2 for all x ∈R2. From
g(7, 2) −g(3, 2) = a1 · 7 + a2 · 2 −(a1 · 3 + a2 · 2) = 4a1 = 8
we conclude that a1 = 2. From
g(7, 5) −g(3, 2) = a1 · 7 + a2 · 5 −(a1 · 3 + a2 · 2) = 4a1 + 3a2 = 8 + 3a2 = 5
we conclude that a2 = −1. Hence g : R2 →R, x 7→(2, −1) · x.
(b) Consider ˆg : R2 →R, x 7→g(x) + 2, where g is the linear function from (a).
How does the value of ˆg change if x changes
(i) from (−3, 0) to (2, 1)?
(ii) from (2, 5) to (1, 3)?
Solution: The change dy in the value of ˆg if its variables change by dx is given by
dy = (2, −1) · dx.
(i) Here, dx = (2, 1) −(−3, 0) = (5, 1) and thus dy = (2, −1) · (5, 1) =
10 −1 = 9.
(ii) Here, dx = (1, 3) −(2, 5) = (−1, −2) and thus dy = (2, −1) · (−1, −2) =
−2 + 2 = 0.
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
