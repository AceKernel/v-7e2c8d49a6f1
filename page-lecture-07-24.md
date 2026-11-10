# Lecture 7: Converse proof

PDF page 24 of 30; printed slide 24.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=24) | [Previous](page-lecture-07-23.md) | [Next](page-lecture-07-25.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
“⇐”: Now suppose that hyp(f ) is convex. We want to show that f is concave.
Take x1, x2 ∈S and let λ ∈[0, 1]. We have to show that
λf (x1) + (1 −λ)f (x2) ≤f (λx1 + (1 −λ)x2).
Since x1, x2 ∈S, (x1, f (x1)), (x2, f (x2)) ∈hyp(f ). Because hyp(f ) is convex,
λ(x1,f (x1)) + (1 −λ)(x2, f (x2))
= (λx1 + (1 −λ)x2, λf (x1) + (1 −λ)f (x2)) ∈hyp(f )
Thus by the definition of a hypograph:
λf (x1) + (1 −λ)f (x2) ≤f (λx1 + (1 −λ)x2)
Therefore, f is concave.
ECON 2050 – Convexity
24 / 30
```
