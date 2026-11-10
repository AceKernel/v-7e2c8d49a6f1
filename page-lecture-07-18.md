# Lecture 7: Composition theorems

PDF page 18 of 30; printed slide 18.

[Page map](map-lecture-07.md) | [Original PDF page](lecture-07.pdf#page=18) | [Previous](page-lecture-07-17.md) | [Next](page-lecture-07-19.md)

Topics: convexity.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Theorem
Let S ⊆Rn be convex, and f is a function from S to R.
1 If f is convex [concave] then −f : S →R, x ↦→−f (x) is concave [convex].
2 If f is convex [concave] and g : R →R is a convex [concave] and increasing function,
then g ◦f is convex [concave].
Proof: Part 1 follows directly from the definition, because minus sign reverses inequalities; for
part 2, just apply the definition twice and use the fact that g is increasing to “pass” the
inequality.
Warning: If g is not increasing, part 2 need not be true. E.g.,
f (x) = x2, is convex; g(y) = −y is convex but not increasing.
But g ◦f : R →R, given by g(f (x)) = −x2 is not convex.
ECON 2050 – Convexity
18 / 30
```
