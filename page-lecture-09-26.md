# Lecture 9: Free primal variables and dual equalities

PDF page 26 of 26; printed slide 26.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=26) | [Previous](page-lecture-09-25.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
2. What happens to the dual if some variables can also take negative values?
Recall that if we interpret the variable xj as running activity j, xj ≥0 means that this
activity must be run at a non-negative level.
In this case, the dual constraint for variable xj: ∑︁m
i=1 aijyi ≥ci.
Inutuitively, this means that the marginal benet from running activity j, cj, the j-th entry
of c, must be no more than the imputed marginal cost of running this activity, ∑︁m
i=1 aijyi.
Without the nonnegativity constraint, it can't be that ∑︁m
i=1 aijyi > ci: otherwise one
would let xi →−∞to get innite prots, which makes no sense.
Thus, we should expect the dual constraint for variable xj to be ∑︁m
i=1 aijyi = ci.
An implication is that the dual of the linear program max{c · x : Ax ≤b} is
min y · b
s.t.
yA = c, y ≥0,
and the dual of the linear program max{c · x : Ax = b} is
min y · b
s.t.
yA = c.
These can be derived using the tricks on slide 7.
ECON 2050  Optimization II
26 / 26
```
