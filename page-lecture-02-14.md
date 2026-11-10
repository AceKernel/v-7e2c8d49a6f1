# Lecture 2: A discontinuous rational example

PDF page 14 of 33; printed slide 14.

[Page map](map-lecture-02.md) | [Original PDF page](lecture-02.pdf#page=14) | [Previous](page-lecture-02-13.md) | [Next](page-lecture-02-15.md)

Topics: continuity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: Consider the function f : R2 →R with
f (x1, x2) =
{︄x1x2
x2
1 +x2
2
if (x1, x2) ̸= (0, 0)
0
if (x1, x2) = (0, 0)
We show that it is discontinuous at (0, 0).
The sequence (ˆxn) = ( 1
n, 0) converges to (0, 0). Since
f (ˆxn) = f
(︃1
n, 0
)︃
=
1
n · 0
(︁1
n
)︁2 + 02 = 0,
∀n,
the sequence (f (ˆxn)) converges to 0.
(˜xn) = ( 1
n, 1
n) also converges to (0, 0), but f (˜xn) →1
2 as
f (˜xn) = f
(︃1
n, 1
n
)︃
=
1
n · 1
n
(︁1
n
)︁2 +
(︁1
n
)︁2 = 1
2,
∀n.
Therefore, we cannot have have f (xn) →0 for all (xn) such that xn →(0, 0).
ECON 2050 – Basic Real Analysis II
14 / 33
```
