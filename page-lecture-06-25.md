# Lecture 6: Payoff matrix

PDF page 25 of 26; printed slide 25.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=25) | [Previous](page-lecture-06-24.md) | [Next](page-lecture-06-26.md)

Topics: Cones, Farkas and feasibility.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
We now have an economy with three assets (stock, bond, call option) and two possible
scenarios; that is, m = 3 and n = 2. The payoff matrix A can be written as
⎛
⎝
uS0
dS0
rB
rB
max {0, uS0 −K}
max {0, dS0 −K}
⎞
⎠.
If p = (p1, p2, p3) is the vector of prices then p1 = S0, p2 = B and p3 is the price of the call
option we wish to determine.
Since it’s reasonable to assume that there is no arbitrage opportunities in the market, the
arbitrage theorem implies the existence of non-negative π1, π2 such that
⎛
⎝
uS0
dS0
rB
rB
max {0, uS0 −K}
max {0, dS0 −K}
⎞
⎠
(︃π1
π2
)︃
=
⎛
⎝
S0
B
p3
⎞
⎠.
ECON 2050 – Linear Algebra II
25 / 26
```
