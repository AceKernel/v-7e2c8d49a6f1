# Lecture 11: KKT candidate procedure

PDF page 9 of 25; printed slide 9.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=9) | [Previous](page-lecture-11-08.md) | [Next](page-lecture-11-10.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
If we can use the extreme value theorem to conclude that a solution exists, similar to the
previous lecture, we have a useful cookbook procedure for solving non-linear programs with
non-negative variables:
We rst check if all constraint functions are ane. If so,
Write down the KKT conditions.
Every x that (together with some λ) satises the KKT conditions is a candidate solution.
The candidates at which the value of the objective function are the largest are the
solutions.
If not:
Check whether the set of gradients of the constraint functions is linearly independent;
identify the points at which it is not (note that the non-negativity constraints x ≥0 also
need to be considered).
Write down the KKT conditions.
Every x that violates the linear independence condition or that (together with some λ)
satises the KKT conditions is a candidate solution.
The candidates at which the value of the objective function are the largest are the
solutions.
ECON 2050  Optimization IV
9 / 25
```
