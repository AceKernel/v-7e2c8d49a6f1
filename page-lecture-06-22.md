# Lecture 6: Arbitrage theorem illustration

PDF page 22 of 26; printed slide 22.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=22) | [Previous](page-lecture-06-21.md) | [Next](page-lecture-06-23.md)

Topics: Cones, Farkas and feasibility.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The discussion above gives rise to the following famous result in finance.
Theorem (Arbitrage Theorem)
Let A be an m × n payoff matrix, and let p denote the vector of (relative) asset prices. Exactly
one of the following statements holds:
(a) There exists an investment portfolio y ∈Rm such that yA ≥0 and y · p < 0.
(b) There is a probability vector π ∈Rn
+ (with ∑︁n
j=1 πj = 1) such that p = Aπ.
Intuitively, the theorem states that
either the expected value of all possible assets is the same and equal to their prices,
or it is possible to create an arbitrage portfolio at a strictly negative cost that guarantees
a non-negative return for every possible scenario,
but not both. In other words, no arbitrage opportunities implies that market is “fair” in the
sense that all assets are fairly priced.
ECON 2050 – Linear Algebra II
22 / 26
```
