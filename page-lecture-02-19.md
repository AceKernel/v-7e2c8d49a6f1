# Lecture 2: Composition example

PDF page 19 of 33; printed slide 19.

[Page map](map-lecture-02.md) | [Original PDF page](lecture-02.pdf#page=19) | [Previous](page-lecture-02-18.md) | [Next](page-lecture-02-20.md)

Topics: continuity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: f : R2 →R, x ↦→x2
1 + x2
2 is continuous.
Proof: The trick is to observe that f = (pr1)2 + (pr2)2:
Recall that pri : R2 →R, x ↦→pri(x) = xi
Hence pri · pri, or, more succinctly, (pri)2 is the function
(pri)2 : R2 →R, x ↦→x2
i ,
and
(pr1)2 + (pr2)2 : R2 →R, x ↦→((pr1)2(x) + (pr2)2(x)) = x2
1 + x2
2.
Therefore, (pr1)2 + (pr2)2 equals f . By the previous theorems,
pri is continuous, and therefore,
pr2
i is continuous, and therefore,
(pr1)2 + (pr2)2 is continuous (that is, f is continuous!)
Alternatively, we can prove that f : R2 →R, x ↦→x2
1 + x2
2 is continuous by realizing that
f = g ◦pr1 + g ◦pr2 for g : R →R, x ↦→x2.
ECON 2050 – Basic Real Analysis II
19 / 33
```
