# Lecture 6: Nonnegative solutions

PDF page 4 of 26; printed slide 4.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=4) | [Previous](page-lecture-06-03.md) | [Next](page-lecture-06-05.md)

Topics: farkas.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Non-negative solutions
In economics, finance, and business, oftentimes it doesn’t make sense for the relevant
quantities to take negative values.
For example, quantities of consumption, capital, labor, assets, to name a few.
Therefore, we sometimes wish to understand whether we can find a non-negative solution to
a system of linear equations, or no solution exists.
More formally, we wish to find a x ∈Rn with x ≥0 such that Ax = b or show that no
such x exists.
Observe that if b = 0, we can just let x = 0, so we assume that b ̸= 0 henceforth.
The problem can be framed as follows: can b be expressed as a non-negative linear
combination of the columns of A; that is, do there exist x1, x2, . . . , xn ≥0 such that
b = x1a1 + x2a2 + . . . + xnan.
ECON 2050 – Linear Algebra II
4 / 26
```
