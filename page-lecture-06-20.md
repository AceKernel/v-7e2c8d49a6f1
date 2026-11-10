# Lecture 6: Payoff-matrix model

PDF page 20 of 26; printed slide 20.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=20) | [Previous](page-lecture-06-19.md) | [Next](page-lecture-06-21.md)

Topics: Cones, Farkas and feasibility.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
To formally model arbitrage, suppose there are m possible assets whose payoff depends on a
scenario that realizes in the future, and there are n possible scenarios.
Let aij be the payoff from one share of asset i in scenario j; the payoff matrix A
summarizes all possible payoffs:
A =
⎛
⎜
⎜
⎜
⎝
a11
a12
. . .
a1n
a21
a22
. . .
a2n
...
...
...
...
am1
am2
. . .
amn
⎞
⎟
⎟
⎟
⎠
A portfolio of assets is represented by a vector y ∈Rm where the i-th component, yi,
represents the amount of asset i held.
yi > 0 represents buying asset i, and yi > 0 represents selling it.
“No arbitrage” requires that there doesn’t exist a portfolio with a strictly negative cost that
pays off non-negative amounts in every scenario.
ECON 2050 – Linear Algebra II
20 / 26
```
