# Lecture 2: Continuity of composition

PDF page 18 of 33; printed slide 18.

[Page map](map-lecture-02.md) | [Original PDF page](lecture-02.pdf#page=18) | [Previous](page-lecture-02-17.md) | [Next](page-lecture-02-19.md)

Topics: continuity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Let D ⊆Rk and f : D →Rm. Let g : E →Rl, where f (D) ⊆E. Then we define the
composition of f with g as
g ◦f : D →Rl, x ↦→g(f (x))
Theorem
Let D ⊆Rk and f : D →Rm be continuous at x ∈D. Let g : E →Rl be continuous at
f (x) ∈E, where f (D) ⊆E. Then g ◦f : D →Rl is continuous at x.
Proof: Let (xn) be an arbitrary sequence contained in D converging to x.
By the continuity of f at x, f (xn) →f (x).
By the continuity of g at f (x), g(f (xn)) →g(f (x)).
This implies, by definition, that g ◦f is continuous at x.
The theorems we just discussed can be very powerful in proving continuity.
ECON 2050 – Basic Real Analysis II
18 / 33
```
