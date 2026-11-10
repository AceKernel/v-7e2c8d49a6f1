# Lecture 10: The direction linear program

PDF page 8 of 28; printed slide 8.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=8) | [Previous](page-lecture-10-07.md) | [Next](page-lecture-10-09.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Because x∗maximizes f on C, the following maximization problem must have a solution h = 0:
max
h
f (x∗) + ∇f (x∗) · h
subject to
gi(x∗) + ∇gi(x∗) · h ≤0 for all i = 1, . . . , m.
Note that dropping the constant terms of the objective functions doesn't aect the solutions,
and therefore the problem above is equivalent to the following linear program:
max
h
∇f (x∗) · h
subject to
∇gi(x∗) · h ≤−gi(x∗) for all i = 1, . . . , m.
If this still doesn't seem familiar to you, let c = ∇f (x ∗),
A =
⎛
⎜
⎜
⎜
⎝
∇g1(x∗)
∇g2(x∗)
...
∇gm(x∗)
⎞
⎟
⎟
⎟
⎠,
and
b =
⎛
⎜
⎜
⎜
⎝
−g1(x∗)
−g2(x∗)
...
−gm(x∗)
⎞
⎟
⎟
⎟
⎠,
the problem can be written as max c · h subject to Ah ≤b.
ECON 2050  Optimization III
8 / 28
```
