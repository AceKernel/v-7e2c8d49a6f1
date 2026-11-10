# Tutorial 10, Problem 4: Parameter-dependent disk constraint: extra practice

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-10-solutions.md) | [Original PDF](tutorial-10-solutions.pdf)

Topics: lagrange.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 6

[Original page](tutorial-10-solutions.pdf#page=6)

```text
Problem 4 (Extra Practice Problem)
Consider the maximization problem
max
(x,y)∈R2 2 −(x −1)2 −ey2
subject to
x2 + y2 ≤a.
Write down the Lagrange conditions, then find the only point that satisfies the Lagrange
conditions.
(Hint. Distinguishing between the cases a ∈(0, 1) and a ≥1.)
Solution: The Lagrange conditions are
−2(x −1) −2λx = 0
−2yey2 −2λy = 0
x2 + y2 ≤a
λ ≥0
λ(x2 + y2 −a) = 0
The first two equations can be simplified to
(x −1) + λx = 0,
(1)
2y(ey2 + λ) = 0.
(2)
We analyze the solution by considering two cases based on the complementary slackness
condition, namely the last equation in the Lagrange conditions.
Case 1: The constraint is not binding (λ = 0).
If λ = 0, the complementary slackness
condition is satisfied.
• From equation (2): 2y(ey2 + 0) = 0 =⇒2yey2 = 0. Since ey2 > 0, we must have
y = 0.
• From equation (1): (x −1) + 0 · x = 0 =⇒x −1 = 0 =⇒x = 1.
6
```

## PDF page 7

[Original page](tutorial-10-solutions.pdf#page=7)

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
