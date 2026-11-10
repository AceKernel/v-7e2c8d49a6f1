# Lecture 1: Convergence tails

PDF page 15 of 30; printed slide 15.

[Page map](map-lecture-01.md) | [Original PDF page](lecture-01.pdf#page=15) | [Previous](page-lecture-01-14.md) | [Next](page-lecture-01-16.md)

Topics: sequences.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The idea of convergence is that the tail of a sequence approximates its limit to any desired
degree of accuracy.
Some initial finitely many terms of the sequence may be quite apart from its limit, but
eventually all terms of the sequence accumulates around this limit.
To see this, consider a sequence (xn) defined as
xn =
{︃n
if n ≤100;
1
n−100
if n > 100.
To show that limn→∞xn = 0, we need to pick N large enough; in fact, we need to pick
N > (1/ε) + 100.
So although real sequences (1/n) and xn appear to be quite different in their first 100
terms, they have the same long-run behavior: they both converge to 0.
That is, the initial terms of the sequence have no say on the behavior of the tail of the
sequence.
ECON 2050 – Basic Real Analysis I
15 / 30
```
