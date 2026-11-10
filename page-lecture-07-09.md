# Lecture 7: Convex functions: definition

PDF page 9 of 30; printed slide 9.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=9) | [Previous](page-lecture-07-08.md) | [Next](page-lecture-07-10.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Convex and Concave Functions (SB Chapter 21.1)
Definition
Let S ⊆Rn be convex. A function f : S →R is convex (on S) if ∀x, y ∈S, ∀λ ∈[0, 1]
f (λx + (1 −λ)y) ≤λf (x) + (1 −λ)f (y).
The function is strictly convex (on S) if ∀x, y ∈S such that x ̸= y, ∀λ ∈(0, 1),
f (λx + (1 −λ)y) < λf (x) + (1 −λ)f (y).
A function is convex if for all x and y, the graph of the function over the line segment
between x and y lies below the line segment between the points (x, f (x)) and (y, f (y)).
ECON 2050 – Convexity
9 / 30
```
