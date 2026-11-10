# Tutorial 7, Problem 1: Convexity of sublevel sets from the definition

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-07-solutions.md) | [Original PDF](tutorial-07-solutions.pdf)

Topics: convexity.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 1

[Original page](tutorial-07-solutions.pdf#page=1)

```text
Problem 1
Show that if g : R2 →R is a convex function and b ∈R then S = {(x, y) ∈R2 :
g(x, y) ≤b} is a convex set.
Solution: We have to show that if (x, y) ∈S, (x′, y′) ∈S and λ ∈[0, 1], then λ(x, y) + (1 −
λ)(x′, y′) ∈S. So let (x, y) ∈S, (x′, y′) ∈S and λ ∈[0, 1].
• (x, y) ∈S implies g(x, y) ≤b and thus
λg(x, y) ≤λb
(1)
• (x′, y′) ∈S implies g(x′, y′) ≤b and thus
(1 −λ)g(x′, y′) ≤(1 −λ)b
(2)
Thus
g(λ(x, y) + (1 −λ)(x′, y′)) ≤λg(x, y) + (1 −λ)g(x′, y′)
≤λb + (1 −λ)b = b,
where the first inequality follows from the convexity of g and the second inequality from
(1) and (2). But g(λ(x, y) + (1 −λ)(x′, y′)) ≤b means that λ(x, y) + (1 −λ)(x′, y′) ∈S.
This is what we wanted to show. Thus S is convex.
Note. S = {(x, y) ∈R2 : g(x, y) ≤b} is called the lower contour set of g for level b.
Similarly, S′ = {(x, y) ∈R2 : h(x, y) ≥a}, which is called the upper contour set of h for
level a. If h : R2 →R is a concave function and a ∈R then S′ is a convex set for every
a ∈R.
```
