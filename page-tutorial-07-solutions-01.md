# Tutorial 7 solutions: P1: Convexity of sublevel sets from the definition; P2: Convexity of a separable sum

PDF page 1 of 5.

[Page map](map-tutorial-07-solutions.md) | [Original PDF page](tutorial-07-solutions.pdf#page=1) | [Next](page-tutorial-07-solutions-02.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
Tutorial 7 Solution
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
