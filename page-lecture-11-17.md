# Lecture 11: Proof by convexity and concavity

PDF page 17 of 25; printed slide 17.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=17) | [Previous](page-lecture-11-16.md) | [Next](page-lecture-11-18.md)

Topics: convexity, lagrange, kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Proof: Denote the constraint set by C ≡{x ∈S : gi(x) ≤0 for i = 1, . . . , m}.
Recall the alternative interpretation of the rst equality in the Lagrange conditions: it is the
rst-order condition of the Lagrangian
L(x, λ∗) = f (x) −λ∗
1g1(x) −λ∗
2g2(x) −· · · −λ∗
mgm(x).
Note that we are taking λ∗= (λ∗
1, . . . , λ∗
m) as constants here so L is only a function of x.
Because for each i = 1, . . . , m, gi is convex, −gi is concave. Therefore, L, as the sum of
concave functions, is also concave. Consequently, since x ∗is a critical point of L, it maximizes
L on S.
Since C ⊆S, x∗also maximizes L on C, meaning that L(x ∗, λ∗) ≥L(x, λ∗) for all x ∈C.
Then
f (x∗) = L(x∗, λ∗) ≥L(x, λ∗) ≥f (x)
for all x ∈C, where the equality follows from complementary slackness (which implies that
λ∗
1g1(x∗) −λ∗
2g2(x∗) −· · · −λ∗
mgm(x∗) = 0), and the second inequality holds because λ∗
i ≥0
and gi(x) ≤0 for each i = 1, . . . , m. Thus, x∗is a solution to the maximization problem.
ECON 2050  Optimization IV
17 / 25
```
