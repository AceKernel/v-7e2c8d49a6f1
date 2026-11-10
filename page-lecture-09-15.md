# Lecture 9: Farkas proof of strong duality

PDF page 15 of 26; printed slide 15.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=15) | [Previous](page-lecture-09-14.md) | [Next](page-lecture-09-16.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
A proof of the duality theorem
Suppose that the primal has a solution; the argument starting from the dual having a solution
is analogous. By weak duality, V ≤W ; it suces to show that V ≥W .
If there exists a vector x ≥0 such that Ax ≤b and c · x ≥W , then we have V ≥W .
In other words, it suces to show that the system of inequalities c · x ≥W , Ax ≤b, and
x ≥0 has a solution. Also, c · x ≥W is equivalent to −c · x ≤−W .
Suppose, toward contrary, that the system −c · x ≤−W , Ax ≤b, and x ≥0 has no
solution; equivalently, the system
(︃A
−c
)︃
x ≤
(︃b
−W
)︃
has no non-negative solution.
Then its Farkas alternative
(︁
y
λ
)︁(︃A
−c
)︃
≥0,
(︁
y
λ
)︁(︃b
−W
)︃
< 0,
and
(︁
y
λ
)︁
≥0.
must have a solution.
ECON 2050  Optimization II
15 / 26
```
