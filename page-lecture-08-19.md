# Lecture 8: Strictly increasing transformations

PDF page 19 of 25; printed slide 19.

[Page map](map-lecture-08.md) | [Original PDF page](lecture-08.pdf#page=19) | [Previous](page-lecture-08-18.md) | [Next](page-lecture-08-20.md)

Topics: unconstrained.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The following result is useful for calculating (global or local) extrema since it allows us to
simplify the optimization problem.
Proposition
If h : R →R is an increasing function, D ⊆Rn, g : D →R and x is a maximum [minimum] of
g, then x is also a maximum [minimum] of h ◦g. If h : R →R is strictly increasing, the
maxima [minima] of h ◦g and g coincide.
Proof idea: compositing with an increasing function preserves maximality [minimality].
Example: Instead of minimizing
f (x, y) = ex2+y2,
we can minimize g(x, y) = x2 + y2  since h(z) = ez is strictly increasing and f = h ◦g, the
minima of f and g coincide.
ECON 2050  Optimization I
19 / 25
```
