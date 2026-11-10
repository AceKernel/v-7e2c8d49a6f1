# Lecture 10: Complementary slackness

PDF page 2 of 28; printed slide 2.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=2) | [Previous](page-lecture-10-01.md) | [Next](page-lecture-10-03.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Complementary slackness
Theorem
If x∗is a solution to the primal and y ∗is a solution to the dual. Then
1 y∗
i > 0 implies ∑︁
j aijx∗
j = bi;
2 ∑︁n
j=1 aijx∗
j < bi implies y ∗
i = 0;
3 x∗
j > 0 implies ∑︁m
i=1 aijy∗
i = cj;
4 ∑︁m
i=1 aijy∗
i > cj implies x∗
j = 0.
Interpretation:
1 y∗
i > 0 means that the marginal value of resource i is strictly positive, and therefore at the
optimum all the available stock of resource i must be used.
2 ∑︁n
j=1 aijx∗
j < bi means that not all available stock of resource i is used, then it must be
that the marginal value of resource i, y ∗
i , is zero.
ECON 2050  Optimization III
2 / 28
```
