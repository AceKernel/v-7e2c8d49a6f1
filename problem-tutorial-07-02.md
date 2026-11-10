# Tutorial 7, Problem 2: Convexity of a separable sum

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-07-solutions.md) | [Original PDF](tutorial-07-solutions.pdf)

Topics: convexity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-07-solutions.pdf#page=1)

```text
Problem 2
Suppose f : R2 →R can be written as
f(x, y) = g(x) + h(y),
where both g and h are convex functions of one variable. Show that f is also convex.
Solution: To show that f is convex, take any (x′, y′), (x′′, y′′) ∈R2 and λ ∈[0, 1]. Now
f(λ(x′, y′) + (1 −λ)(x′′, y′′)) = f(λx′ + (1 −λ)x′′, λy′ + (1 −λ)y′′)
= g(λx′ + (1 −λ)x′′) + h(λy′ + (1 −λ)y′′).
Because both g and h are convex,
g(λx′ + (1 −λ)x′′) ≤λg(x′) + (1 −λ)g(x′′),
1
```

## PDF page 2

[Original page](tutorial-07-solutions.pdf#page=2)

```text
ECON 2050
S2 2026
and
h(λy′ + (1 −λ)y′′) ≤λh(y′) + (1 −λ)h(y′′).
Thus,
f(λ(x′, y′) + (1 −λ)(x′′, y′′)) = g(λx′ + (1 −λ)x′′) + h(λy′ + (1 −λ)y′′)
≤λg(x′) + (1 −λ)g(x′′) + λh(y′) + (1 −λ)h(y′′)
= λ[g(x′) + h(y′)] + (1 −λ)[g(x′′) + h(y′′)]
= λf(x′, y′) + (1 −λ)f(x′′, y′′)
By definition, f(x, y) is convex.
```
