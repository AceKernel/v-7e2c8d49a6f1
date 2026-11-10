# Lecture 9: Marginal resource values

PDF page 22 of 26; printed slide 22.

[Page map](map-lecture-09.md) | [Original PDF page](lecture-09.pdf#page=22) | [Previous](page-lecture-09-21.md) | [Next](page-lecture-09-23.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Another way to understand the dual is to ask: would additional resource be valuable, and if so
just how much?
The solution of the dual is (y ∗
1 , y∗
2 , y∗
3 ) = (1
2, 1
2, 0).
Note that the constraint on the fridge storage space x2 ≤6
5 is slack at the primal solution
(x∗
1, x∗
2) = (1, 1).
In other words, as long as the fridge storage space is no less than 1, the solution
(x∗
1, x∗
2) = (1, 1) is still revenue-maximizing.
Therefore, for slight changes in the fridge storage space, the value of y ∗
3 gives us the
change in optimal objective function value, namely zero.
Let's now turn to a binding constraint, say the labor constraint, and suppose the units of
available labor increases by very little, say 0.1 (so 4 becomes 4.1).
One can verify that after this change, the primal solution is still at the intersection of the
(new) labor boundary x1 + 3x2 = 4.1 and production capacity boundary x1 + x2 = 2,
which is (0.95, 1.05), and the new optimal value is 3.05 instead of 3.
But 3.05 = 3 + y ∗
1 · (change in available labor) = 3 + 0.1y ∗
1 .
ECON 2050  Optimization II
22 / 26
```
