# Lecture 5: Span example

PDF page 5 of 26; printed slide 5.

[Page map](map-lecture-05.md) | [Original PDF page](lecture-05.pdf#page=5) | [Previous](page-lecture-05-04.md) | [Next](page-lecture-05-06.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: Consider the set of vectors S = {(0, 1), (2, 1)}.
span(S) is the set of all linear combinations of the vectors in S. Since S contains two vectors
x1 = (0, 1) and x2 = (2, 1), the span is
span(S) = {a1(0, 1) + a2(2, 1) : a1, a2 ∈R}
= {(0 · a1 + 2 · a2, 1 · a1 + 1 · a2) : a1, a2 ∈R}
= {(2a2, a1 + a2) : a1, a2 ∈R}
But then any vector x = (x1, x2) ∈R2 can be written as (2a2, a1 + a2) by letting a2 = x1/2
and a1 = x2 −x1/2. Thus, span(S) = R2.
ECON 2050 – Linear Algebra I
5 / 26
```
