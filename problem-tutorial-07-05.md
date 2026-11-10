# Tutorial 7, Problem 5: Strict convexity of a square from the definition

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-07-solutions.md) | [Original PDF](tutorial-07-solutions.pdf)

Topics: convexity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 3

[Original page](tutorial-07-solutions.pdf#page=3)

```text
Problem 5
Prove from the definition of a strictly convex function and without using any theorem
about convex functions that f(x) = x2 is strictly convex.
3
```

## PDF page 4

[Original page](tutorial-07-solutions.pdf#page=4)

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
```
