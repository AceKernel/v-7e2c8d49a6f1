# Lecture 2: Componentwise continuity

PDF page 17 of 33; printed slide 17.

[Page map](map-lecture-02.md) | [Original PDF page](lecture-02.pdf#page=17) | [Previous](page-lecture-02-16.md) | [Next](page-lecture-02-18.md)

Topics: continuity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem
Let D ⊆Rk and f = (f1, . . . , fm) : D →Rm. Then f is continuous at x ∈D if and only if for
every i = 1, . . . , m, fi is continuous at x ∈D.
This is because a theorem from the previous lecture (Slide 23) indicates that f (xn) →f (x∗) if
and only if fi(xn) →fi(x∗) for each i = 1, . . . , k.
Theorem
For every i = 1, . . . , k, the i-th projection pri : Rk →R, x ↦→pri(x) = xi is a continuous
function.
This is because if xn →x∗, then for any i = 1, . . . , k, xin →x∗
i , where xin and x∗
i are the i-th
coordinate of xn and x∗, respectively. Alternatively, one may also consider f : Rm →Rm given
by f (x) = x, and then use the theorem above.
ECON 2050 – Basic Real Analysis II
17 / 33
```
