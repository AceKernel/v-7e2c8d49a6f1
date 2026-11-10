# Lecture 9: Bounding a primal objective

PDF page 10 of 26; printed slide 10.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=10) | [Previous](page-lecture-09-09.md) | [Next](page-lecture-09-11.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Going back to our bakery example,
max
x1 + 2x2
s.t.
x1 + 3x2 ≤4,
x1 + x2 ≤2,
x1, x2 ≥0.
In an attempt to solve this problem, we can produce upper bounds on its optimal value V :
Since x1 + 2x2 ≤x1 + 3x2 ≤4, we know V ≤4.
Since x1 + 2x2 ≤(2/3)(x1 + 3x2) + (1/3)(x1 + x2) ≤(2/3)4 + (1/3)2 = 10/3, V ≤10/3.
Since x1 + 2x2 ≤(1/2)(x1 + 3x2) + (1/2)(x1 + x2) ≤(1/2)4 + (1/2)2 = 3, we know
V ≤3.
In each of these cases we take a non-negative linear combination of the constraints, looking for
better and better upper bounds on the maximum possible value of the objective function
x1 + 2x2.
ECON 2050  Optimization II
10 / 26
```
