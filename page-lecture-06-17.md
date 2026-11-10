# Lecture 6: Deriving an inequality alternative

PDF page 17 of 26; printed slide 17.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=17) | [Previous](page-lecture-06-16.md) | [Next](page-lecture-06-18.md)

Topics: farkas.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: Let us derive the Farkas alternative for the system [Ax ≤b and x ≥0].
Recall that we can add a slack variable s1 ≥0 to the first inequality ∑︁n
j=1 a1jxj ≤b1 to
convert it to an equality ∑︁n
j=1 a1jxj + s1 = b1.
We do this to all inequalities, and let s ≡(s1, s2, . . . , sm) be the slack vector; evidently,
s ≥0.
Therefore, “whether we can find x ≥0 such that Ax ≤b” is equivalent to “whether we
can find x ≥0 and s ≥0 such that Ax + s = b.”
Let I denote the (m × m) identity matrix, which is a matrix whose diagonal entries are 1
and off-diagonal entries are 0. It is not hard to verify that for any c ∈Rm, Ic = cI = c.
Thus, Ax + s = b is equivalent to Ax + Is = b.
Set B ≡[A|I], and let z ≡(x, s) = (x1, x2, . . . , xn, s1, s2, . . . , sm), and we can write the
system [Ax + Is = b, x ≥0, and s ≥0] as [Bz = b and z ≥0].
ECON 2050 – Linear Algebra II
17 / 26
```
