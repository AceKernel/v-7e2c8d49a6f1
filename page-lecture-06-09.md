# Lecture 6: Proof of Farkas lemma

PDF page 9 of 26; printed slide 9.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=9) | [Previous](page-lecture-06-08.md) | [Next](page-lecture-06-10.md)

Topics: farkas, graphs.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem (Farkas Lemma)
Let A be an m × n matrix, b ∈Rm, and F = {x ∈Rn : Ax = b, x ≥0}. Then either F ̸= ∅
or there exists y ∈Rm such that yA ≥0 and y · b < 0, but not both.
(Algebraic) intuition:
Take any linear combination of the equations in Ax = b to get yAx = y · b.
Suppose the first system has non-negative solution, then it must also be a solution to the
second.
If we can choose y so that yA ≥0 and y · b < 0, we find that the left-hand side of the
single equation yAx = y · b is at least zero while the right-hand side is strictly negative, a
contradiction.
Thus, the first system cannot have a non-negative solution.
ECON 2050 – Linear Algebra II
9 / 26
```
