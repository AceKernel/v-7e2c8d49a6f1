# Lecture 9: Maximisation standard form, binding and slack

PDF page 7 of 26; printed slide 7.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=7) | [Previous](page-lecture-09-06.md) | [Next](page-lecture-09-08.md)

Topics: linear-programming.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
General setup and terminology
Every linear programming problem can be written in the following standard form:
max c · x
s.t.
Ax ≤b
x ≥0
Or more compactly, max{c · x : Ax ≤b, x ≥0}.
If xj doesn't have to be non-negative, substitute xj = x+
j −x−
j , where x+
j , x−
j
≥0.
If the objective is min c · x then replace it with max −c · x.
If the i-th constraint is ∑︁n
j=1 aijxj ≥bi, replace it by −∑︁n
j=1 aijxj ≤−bi.
If the i-th constraint is ∑︁n
j=1 aijxj = bi, replace it by two inequality constraints:
∑︁n
j=1 aijxj ≤bi and −∑︁n
j=1 aijxj ≤−bi.
Suppose ˜x is in the constraint set. Then if a constraint holds with equality, say that this
constraint binds at ˜x; if instead the constraint holds with strict inequality, we say it is slack at
˜x.
ECON 2050  Optimization II
7 / 26
```
