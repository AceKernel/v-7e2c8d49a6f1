# Lecture 4: Multivariable inner functions

PDF page 7 of 25; printed slide 7.

[Page map](map-lecture-04.md) | [Original PDF page](lecture-04.pdf#page=7) | [Previous](page-lecture-04-06.md) | [Next](page-lecture-04-08.md)

Topics: chain-hessian.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The theorem above also suggests a natural generalization of the chain rule to the case where
the “inside functions” are also functions of several variables.
Theorem
Suppose that f : Rk →R is differentiable, and for each j = 1, 2, . . . , k, gj : R →R is
differentiable. Then the function G : Rm →R given by
F(x) ≡f (g1(x), . . . , gk(x))
is differentiable, and for each i = 1, . . . , m,
∂F(x)
∂xi
= f1(g1(x), . . . , gk(x))∂g1(x)
∂xi
+ . . . + fk(g1(x), . . . , gk(x))∂gk(x)
∂xi
,
where xi is the i-th coordinate of x, fj is the partial derivative of f with respect to its j-th
coordinate.
ECON 2050 – Basic Real Analysis IV
7 / 25
```
