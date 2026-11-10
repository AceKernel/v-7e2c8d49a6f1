# Lecture 10: Dual of the direction program

PDF page 9 of 28; printed slide 9.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=9) | [Previous](page-lecture-10-08.md) | [Next](page-lecture-10-10.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The dual of the problem max c · h subject to Ah ≤b is
min λ · b
subject to
λA = c and λ ≥0.
Recalling that c = ∇f (x∗),
A =
⎛
⎜
⎜
⎜
⎝
∇g1(x∗)
∇g2(x∗)
...
∇gm(x∗)
⎞
⎟
⎟
⎟
⎠,
and
b =
⎛
⎜
⎜
⎜
⎝
−g1(x∗)
−g2(x∗)
...
−gm(x∗)
⎞
⎟
⎟
⎟
⎠,
the dual can be written as
min
λ −λ1g1(x∗) −λ2g2(x∗) −· · · −λmgm(x∗)
s.t. λ1∇g1(x∗) + λ2∇g2(x∗) + · · · + λm∇gm(x∗) = ∇f (x∗)
λi ≥0 for each i = 1, . . . , m.
ECON 2050  Optimization III
9 / 28
```
