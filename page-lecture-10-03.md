# Lecture 10: Expanded complementary-slackness conditions

PDF page 3 of 28; printed slide 3.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=3) | [Previous](page-lecture-10-02.md) | [Next](page-lecture-10-04.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
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
Interpretation (Continued): Recall from the previous lecture that cj is the marginal benet from
running activity j, and the imputed marginal cost of running activity j is ∑︁m
i=1 aijyi. Then
3 x∗
j > 0 means that the (imputed) marginal cost and marginal benet must equal, as
otherwise xj should be set to 0.
4 ∑︁m
i=1 aijy∗
i > cj means that the (imputed) marginal cost is strictly higher than marginal
benet, so engaging in activity j would incur a loss, hence x ∗
j must be zero.
ECON 2050  Optimization III
3 / 28
```
