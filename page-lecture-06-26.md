# Lecture 6: State prices and binomial pricing

PDF page 26 of 26; printed slide 26.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=26) | [Previous](page-lecture-06-25.md)

Topics: Cones, Farkas and feasibility.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Consider the first two equations:
uS0π1 + dS0π2 = S0
rBπ1 + rBπ2 = B
They have a unique non-negative solution
π1 =
r −d
r(u −d),
and
π2 =
u −r
r(u −d).
Using this solution, we deduce that
p3 = π1 max
{︁
0, uS0 −K
}︁
+ π2 max
{︁
0, dS0 −K
}︁
.
(⋆)
This option pricing formula (⋆) is the discrete (one period) analogue of the celebrated
Black–Scholes formula.
Note that the price of the call option doesn’t depend on the probabilities of either the
good or bad scenario being realized.
ECON 2050 – Linear Algebra II
26 / 26
```
