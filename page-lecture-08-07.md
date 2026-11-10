# Lecture 8: Why an interior optimum has zero gradient

PDF page 7 of 25; printed slide 7.

[Page map](map-lecture-08.md) | [Original PDF page](lecture-08.pdf#page=7) | [Previous](page-lecture-08-06.md) | [Next](page-lecture-08-08.md)

Topics: unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Proof sketch (two variable case):
Suppose f : R2 →R achieves a local maximum at point (x∗
1, x∗
2). Then
∃r > 0, ∀(x1, x2) ∈Br(x∗
1, x∗
2) :
f (x1, x2) ≤f (x∗
1, x∗
2)
Thus, if we keep x2 = x∗
2 xed and dene g : R →R given by g(x1) ≡f (x1, x∗
2),
∀x1 ∈pr1(Br(x∗
1, x∗
2)) :
g(x1) = f (x1, x∗
2) ≤f (x∗
1, x∗
2) = g(x∗
1)
This implies that the one variable function g has a local maximum at x1 = x∗
1, which implies
that g ′(x∗
1) = 0 and therefore
∂f (x∗
1, x∗
2)
∂x1
= 0
Analogously, keeping x1 = x∗
1 xed, we obtain ∂f (x∗
1 ,x∗
2 )
∂x2
= 0.
Changing ≤for ≥demonstrates the same result for a local minimum.
ECON 2050  Optimization I
7 / 25
```
