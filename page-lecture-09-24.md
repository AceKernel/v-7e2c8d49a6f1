# Lecture 9: Primal equalities and free dual multipliers

PDF page 24 of 26; printed slide 24.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=24) | [Previous](page-lecture-09-23.md) | [Next](page-lecture-09-25.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Writing down the dual
The interpretation of the dual allow us to answer the following questions regarding the dual.
1. What happens to the dual if some constraints in the primal hold with = instead of ≤(we
don't need to worry too much about ≥because it can be easily converted to ≤)?
Recall that the dual variable yi for the constraint ∑︁n
j=1 aijxj ≤bi must satisfy yi ≥0.
This is because yi can be interpreted as the marginal value of relaxing this constraint,
which cannot be negative because doing so enlarges the constraint set.
But if the constraint is ∑︁n
j=1 aijxj = bi, as bi increases the constraint set becomes
completely dierent, and therefore the marginal value can be negative.
Thus, the sign of the dual variable for a equality constraint is unconstrained.
An implication is that the dual of the linear program max{c · x : Ax = b, x ≥0} is
min y · b
s.t.
yA ≥c.
ECON 2050  Optimization II
24 / 26
```
