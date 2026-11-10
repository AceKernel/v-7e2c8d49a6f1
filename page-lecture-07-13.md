# Lecture 7: Affine functions are convex and concave

PDF page 13 of 30; printed slide 13.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=13) | [Previous](page-lecture-07-12.md) | [Next](page-lecture-07-14.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Examples:
f (x1, x2) = x1 + x2 is both convex and concave:
Let (x′
1, x′
2), (x′′
1 , x′′
2 ) ∈R2 and λ ∈[0, 1], then
f (λ(x′
1, x′
2) + (1 −λ)(x′′
1 , x′′
2 )) = f (λx′
1 + (1 −λ)x′′
1 , λx′
2 + (1 −λ)x′′
2 )
= λx′
1 + (1 −λ)x′′
1 + λx′
2 + (1 −λ)x′′
2
= λ(x′
1 + x′
2) + (1 −λ)(x′′
1 + x′′
2 )
= λf (x′
1, x′
2) + (1 −λ)f (x′′
1 , x′′
2 )
Thus f is both concave and convex, but neither strictly concave nor strictly convex.
More generally, every affine function f : Rn →R is both convex and concave (exercise).
f1(x) = x2 and f2(x) = ex are strictly convex, f3(x) = ln x and f4(x) = √x are strictly
concave.
ECON 2050 – Convexity
13 / 30
```
