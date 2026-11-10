# Lecture 6: Binomial-model setup

PDF page 24 of 26; printed slide 24.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=24) | [Previous](page-lecture-06-23.md) | [Next](page-lecture-06-25.md)

Topics: Cones, Farkas and feasibility.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
For simplicity, assume a single time period and a market consisting of a stock, a bond, and a
call option on the stock.
Let K be the strike price of the call option and suppose that it can be exercised only at the
end of the time period. Suppose S is the value of the stock at the end of the time period.
If S > K, the option holder will exercise the call option yielding a profit of S −K dollars.
If S ≤K, the option holder will let the call option expire and its value to the holder is
zero.
To summarize, the call option has a payoff of max{0, S −K}.
Suppose that there are only two possible future scenarios, say good and bad.
The good scenario is where the stock goes up by a factor u > 1, and the bad scenario is
where the stock declines by a factor d < 1.
Investing in the bond is risk free, which means that in all cases in the future the value of
the bond goes up by a factor r > 1; we assume that r < u to make the setting interesting.
Let S0 be the initial stock price and B the price of the bond.
ECON 2050 – Linear Algebra II
24 / 26
```
