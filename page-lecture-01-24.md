# Lecture 1: Order and scalar limit results

PDF page 24 of 30; printed slide 24.

[Page map](map-lecture-01.md) | [Original PDF page](lecture-01.pdf#page=24) | [Previous](page-lecture-01-23.md) | [Next](page-lecture-01-25.md)

Topics: sequences.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem
Let (xn)n∈N and (yn)n∈N be sequences with codomain R. If limn→∞xn = x∗∈R and
limn→∞yn = y∗∈R, then
(a) limn→∞(xn · yn) = x∗· y∗
(b) if there exists b ∈R such that xn ≤b for all n ∈N, then x∗≤b.
Proof of part (a) is left as an exercise. See SB Thm 12.3 if you are interested.
Proof of part (b): Suppose, toward a contradiction, that xn ≤b for all n ∈N, but x∗> b.
Choose ε so that 0 < ε < x∗−b (e.g., we can let ε = (x∗−b)/2). Then, b < x∗−ε.
Because xn →x∗, there exists N ∈N such that for all n ≥N,
xn ∈Bε(x∗) = (x∗−ε, x∗+ ε).
This implies that xn ≥b for all n ≥N, a contradiction.
ECON 2050 – Basic Real Analysis I
24 / 30
```
