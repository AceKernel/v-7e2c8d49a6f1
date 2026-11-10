# Lecture 6: Slack, surplus and free-variable conversions

PDF page 16 of 26; printed slide 16.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=16) | [Previous](page-lecture-06-15.md) | [Next](page-lecture-06-17.md)

Topics: farkas.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Below is a cookbook procedure that allows us to convert any inequality system into an
equality system with non-negative variables:
For each inequality of the system, ∑︁n
j=1 aijxj ≤bi, we can add a slack variable to it to
get ∑︁n
j=1 aijxj + si = bi.
For each inequality of the system of the form ∑︁n
j=1 aijxj ≥bi, we can subtract a surplus
variable to it to get ∑︁n
j=1 aijxj −si = bi.
For a variable, xj, that is unrestricted in sign can be replaced by two non-negative
variables zj and z′
j by setting xj = zj −z′
j.
ECON 2050 – Linear Algebra II
16 / 26
```
