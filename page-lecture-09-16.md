# Lecture 9: Completing the duality proof

PDF page 16 of 26; printed slide 16.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=16) | [Previous](page-lecture-09-15.md) | [Next](page-lecture-09-17.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The Farkas alternative can be written as
yA −λc ≥0,
y · b −λW < 0,
y ≥0,
and
λ ≥0;
denote a solution by
(︁
y ∗
λ∗)︁
.
Observe that λ∗> 0: if instead λ∗= 0, the system above reduces to
yA ≥0,
y · b < 0,
and
y ≥0,
which is the Farkas alternative of the system Ax ≥b and x ≥0.
Since it has a solution y ∗, the Farkas lemma implies that the system Ax ≥b and x ≥0
has no solution, violating the assumption that the primal has a solution. Thus, λ∗> 0.
Let ˆy ≡y ∗/λ∗; this is well-dened because λ∗> 0. The system at the top implies
ˆy · A ≥c,
ˆy ≥0,
and
ˆy · b < W ,
showing that ˆy is feasible for the dual and the value of the dual objective function at ˆy is
strictly below W , contradicting the assumption that W is the optimal value of the dual.
ECON 2050  Optimization II
16 / 26
```
