# Lecture 10: Equalities as opposite inequalities

PDF page 23 of 28; printed slide 23.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=23) | [Previous](page-lecture-10-22.md) | [Next](page-lecture-10-24.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Equality constraints
On slide 6, we mentioned that every constraint can be written as a less than or equal to
constraint. Specically,
If the constraint looks like g(x) ≤h(x), we can write it as g(x) −h(x) ≤0.
gi(x) ≥0 can be written as −gi(x) ≤0.
gi(x) = 0 can be replaced by two inequality constraints: gi(x) ≤0 and −gi(x) ≤0.
If all constraint functions are ane, everything works out smoothly. However, if not, we need
to test linear independence of the set of gradients of the binding constraint functions.
The linear independence of that set is sensitive to the representation of the constraint set.
To see why, consider the problem max f (x) subject to g(x) = 0.
This can be written as max f (x) subject to g(x) ≤0 and −g(x) ≤0.
However, both constraints bind, and the set of gradients {∇g(x), −∇g(x)} is linearly
dependent, and therefore we can't use the theorem on slide 15.
ECON 2050  Optimization III
23 / 28
```
