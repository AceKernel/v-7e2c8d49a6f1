# Lecture 4: Second partials of an exponential

PDF page 11 of 25; printed slide 11.

[Page map](map-lecture-04.md) | [Original PDF page](lecture-04.pdf#page=11) | [Previous](page-lecture-04-10.md) | [Next](page-lecture-04-12.md)

Topics: chain-hessian.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: To obtain the second-order partial derivatives of
f : R2 →R, (x, y) ↦→exy,
we first calculate the first-order partial derivatives
∂f (x, y)
∂x
= yexy;
∂f (x, y)
∂y
= xexy
and then differentiate these with respect to x and with respect to y:
∂2f (x, y)
∂x2
=
y2exy;
∂2f (x, y)
∂x∂y
= exy + yxexy = exy(1 + xy)
∂2f (x, y)
∂y2
=
x2exy;
∂2f (x, y)
∂y∂x
= exy + yxexy = exy(1 + xy)
Observe that here, the cross partial derivatives are equal.
ECON 2050 – Basic Real Analysis IV
11 / 25
```
