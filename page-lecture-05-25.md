# Lecture 5: Rank criterion: expressly excluded on this slide

PDF page 25 of 26; printed slide 25.

[Page map](map-lecture-05.md) | [Original PDF page](lecture-05.pdf#page=25) | [Previous](page-lecture-05-24.md) | [Next](page-lecture-05-26.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Sometimes the solvability of a system of linear equations is more conveniently determined by
the following result (will not appear in any assignments or exam):
Theorem
Let A be an m × n matrix of rank r and b ∈Rm. Let r′ be the rank of the augmented matrix
[A | b] and let F = {x ∈Rn : Ax = b}. Then exactly one of the following must be true:
(i) if r′ = r + 1, F = ∅;
(ii) if r′ = r = n, F is a single vector;
(iii) if r = r′ < n, then F contains infinitely many vectors.
r′ = r + 1 implies that b cannot be written as a linear combination of columns of A; i.e.,
b /∈span(A). This means that there doesn’t exist x ∈Rn such that Ax = b, and hence
the system has no solution.
r′ = r means that b can be written as a linear combination of columns of A:
b ∈span(A). Thus, a solution exists. If r = n, there are n equations and n unknowns,
and therefore exactly one solution; if r < n, some equations are “redundant.”
ECON 2050 – Linear Algebra I
25 / 26
```
