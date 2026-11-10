# Tutorial 10 solutions: P4: Parameter-dependent disk constraint: extra practice

PDF page 7 of 7.

[Page map](map-tutorial-10-solutions.md) | [Original PDF page](tutorial-10-solutions.pdf#page=7) | [Previous](page-tutorial-10-solutions-06.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
This gives the candidate point (1, 0). The constraint requires
12 + 02 ≤a =⇒1 ≤a
So, if a ≥1, the point (x∗, y∗, λ∗) = (1, 0, 0) satisfies Lagrange conditions; otherwise it
doesn’t.
Case 2: The constraint is binding (λ > 0).
If λ > 0, the complementary slackness condition
requires x2 + y2 −a = 0.
• From equation (2), 2y(ey2 + λ) = 0. Since λ > 0 and ey2 > 0, their sum is positive.
Therefore, we must have y = 0.
• Substitute y = 0 into the binding constraint: x2 + 02 = a =⇒x = ±√a.
• We use equation (1) to find the valid value for x:
(x −1) + λx = 0 =⇒λ = 1 −x
x
• Since we are in the case where λ > 0, we require 1−x
x
> 0.
– Testing x = √a: We need λ = 1−√a
√a
> 0. Since √a > 0 (for a > 0), this requires
1 −√a > 0 =⇒1 > a.
– Testing x = −√a: We need 1−(−√a)
−√a
> 0, which is 1+√a
−√a > 0. This is never true
as the numerator is positive and the denominator is negative.
The only valid candidate point in this case is (x∗, y∗, λ∗) = (√a, 0, (1/√a −1))), which
satisfies the Lagrange conditions for 0 ≤a < 1.
To summarize,
• If a ≥1, the unique point satisfying the Lagrange conditions is (x∗, y∗, λ∗) = (1, 0, 0)
with a maximum value of 1.
• If 0 ≤a < 1, the unique point satisfying the Lagrange conditions is (x∗, y∗, λ∗) =
(√a, 0, (1/√a −1)).
7
```
