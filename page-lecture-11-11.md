# Lecture 11: Completing the logarithmic example

PDF page 11 of 25; printed slide 11.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=11) | [Previous](page-lecture-11-10.md) | [Next](page-lecture-11-12.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Because λ > 0, by complementary slackness, 6 −x1 −x2 = 0. Therefore,
(x∗
1, x∗
2, λ∗) = (3, 3, 3) satises the KKT conditions.
Now suppose instead x1 = 0. If x2 > 0, by complementary slackness, x2(x1 −λ) = 0
implies λ = x1 = 0.
But then since x2 −λ ≤0, it must be that x2 ≤0, a contradiction. Thus, x∗
2 = λ∗= 0.
Therefore, (x∗
1, x∗
2, λ∗) = (0, 0, 0) also satises the KKT conditions.
Because the objective function is continuous and the constraint set is compact (draw a
picture), by the extreme value theorem a solution exists.
Then since the KKT conditions are necessary, all solutions must be among the points at
which the KKT conditions are satised.
Because the value of the objective function at (x1, x2) = (3, 3) is strictly greater than that
at (0, 0), the unique solution of the problem is (x ∗
1, x∗
2) = (3, 3).
ECON 2050  Optimization IV
11 / 25
```
