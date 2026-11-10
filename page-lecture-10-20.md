# Lecture 10: Existence and complete candidate procedure

PDF page 20 of 28; printed slide 20.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=20) | [Previous](page-lecture-10-19.md) | [Next](page-lecture-10-21.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
If we can use the extreme value theorem to conclude that a solution exists, we have a useful
cookbook procedure for solving non-linear programs:
We rst check if all constraint functions are ane. If so,
Write down the Langrange conditions.
Every x that (together with some λ) satises the Lagrange conditions is a candidate
solution.
The candidates at which the value of the objective function are the largest are the
solutions.
If not:
Check whether the set of gradients of the constraint functions is linearly independent;
identify the points at which it is not.
Write down the Langrange conditions.
Every x that violates the linear independence condition or that (together with some λ)
satises the Lagrange conditions is a candidate solution.
The candidates at which the value of the objective function are the largest are the
solutions.
ECON 2050  Optimization III
20 / 28
```
