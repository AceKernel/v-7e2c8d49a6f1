# Lecture 5: Equality of row and column rank

PDF page 15 of 26; printed slide 15.

[Page map](map-lecture-05.md) | [Original PDF page](lecture-05.pdf#page=15) | [Previous](page-lecture-05-14.md) | [Next](page-lecture-05-16.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem
Let A be an m × n matrix. Then its column rank and row rank coincide.
The formal proof of this result is beyond the scope of this course, but it makes intuitive sense:
Let’s revisit the example of the set of vectors S = {(1, 2, 3), (4, 5, 6)}.
If we interpret each vector in S as a row, we get a matrix
A =
(︃1
2
3
4
5
6
)︃
.
Interpreting each vector in S as a column, we get a matrix
B =
⎛
⎝
1
4
2
5
3
6
⎞
⎠= A⊺.
But the rank of a set of vectors shouldn’t be affected by the way we interpret the vectors.
ECON 2050 – Linear Algebra I
15 / 26
```
