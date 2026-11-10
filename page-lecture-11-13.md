# Lecture 11: Active gradients and qualification

PDF page 13 of 25; printed slide 13.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=13) | [Previous](page-lecture-11-12.md) | [Next](page-lecture-11-14.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The linear independence condition is satised at all relevant points:
▶If exactly 2 constraints bind, then the set of gradients of binding constraint functions is
always linearly independent:
⋆If x = 0 and y = 0, since ∇n1(x, y) = (−1, 0) and ∇n2(x, y) = (0, −1) the set of gradients of
binding constraint functions is
{(−1, 0), (0, −1)} , which is linearly independent
⋆If x = 0 and x2 + y 2 = 2 then y =
√
2 and since ∇g(x, y) = (2x, 2y) and ∇n1(x, y) = (−1, 0),
the set of gradients of constraint functions binding at (x, y) = (0,
√
2) is
{∇g(0,
√
2), ∇n1(0,
√
2)} = {(0, 2
√
2), (−1, 0)},
which is linearly independent.
⋆If y = 0 and x2 + y 2 = 2 then x =
√
2 ∇g(x, y) = (2x, 2y) and ∇n2(x, y) = (0, −1),
the set of gradients of constraint functions binding at (x, y) = (
√
2, 0) is
{∇g(
√
2, 0), ∇n2(
√
2, 0)} = {(2
√
2, 0), (0, −1)},
which is linearly independent.
▶It is not possible that all 3 constraints bind: x = y = 0 implies x 2 + y 2 < 2.
ECON 2050  Optimization IV
13 / 25
```
