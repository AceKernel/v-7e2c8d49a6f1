# Tutorial 7 solutions: P5: Strict convexity of a square from the definition; P6: Intersections of convex sets: extra practice

PDF page 4 of 5.

[Page map](map-tutorial-07-solutions.md) | [Original PDF page](tutorial-07-solutions.pdf#page=4) | [Previous](page-tutorial-07-solutions-03.md) | [Next](page-tutorial-07-solutions-05.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Solution: f is strictly convex if for all x′, x′′ ∈R such that x′ ̸= x′′, and all λ ∈(0, 1),
f(λx′ + (1 −λ)x′′) < λf(x′) + (1 −λ)f(x′′).
So let x′, x′′ ∈R be such that x′ ̸= x′′, and λ ∈(0, 1). Then
f(λx′ + (1 −λ)x′′) = (λx′ + (1 −λ)x′′)2 = λ2(x′)2 + 2λ(1 −λ)x′x′′ + (1 −λ)2(x′′)2
and
λf(x′) + (1 −λ)f(x′′) = λ(x′)2 + (1 −λ)(x′′)2.
Now observe that
λf(x′) + (1 −λ)f(x′′) −f(λx′ + (1 −λ)x′′)
= λ(x′)2 + (1 −λ)(x′′)2 −

λ2(x′)2 + 2λ(1 −λ)x′x′′ + (1 −λ)2(x′′)2
= (λ −λ2)(x′)2 −2λ(1 −λ)x′x′′ +

1 −λ −(1 −λ)2
(x′′)2
= λ(1 −λ)(x′)2 −2λ(1 −λ)x′x′′ + (1 −λ)[1 −(1 −λ)](x′′)2
= λ(1 −λ)

(x′)2 −2x′x′′ + (x′′)2
= λ(1 −λ)(x′ −x′′)2 > 0
where the strict inequality holds since x′ ̸= x′′ and λ ∈(0, 1). Hence f(λx′ + (1 −λ)x′′) <
λf(x′) + (1 −λ)f(x′′) and f is strictly convex.
Problem 6 (Extra Practice Problem)
Apply the result from Problem 1 and the properties of a convex set to demonstrate that
the following sets are convex.
1. S = {(x, y) ∈R2 : y ≥x2, x2 + y2 ≤4, x ≥0, y ≥0}
2. T = {(x, y) ∈R2 : x2 + y2 ≤25, x + y ≥5, y ≥2, x ≥0}
Solution: (Sketch only)
1. S is convex, as it is the intersection of the following sets, all of which are convex:
• S1 = {(x, y) ∈R2 : y ≥x2} (we showed in Problem 3 that it is convex),
• S2 = {(x, y) ∈R2 : y2 + x2 ≤4} (we showed in Problem 3 that it is convex),
• S3 = {(x, y) ∈R2 : −x ≤0} (convex by Problem 1 because f3(x, y) = −x is
affine and thus convex)
• S4 = {(x, y) ∈R2 : −y ≤0} (convex by Problem 1 because f4(x, y) = −y is
affine and thus convex)
Graphically:
4
```
