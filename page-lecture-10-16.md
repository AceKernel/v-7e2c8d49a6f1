# Lecture 10: Active gradients and qualification failure

PDF page 16 of 28; printed slide 16.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=16) | [Previous](page-lecture-10-15.md) | [Next](page-lecture-10-17.md)

Topics: lagrange.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
The trickiness with the linear independence test is that we can't determine which constraints
are binding until we have identied candidate solutions from the Lagrange conditions.
What we usually do instead is to test the linear independence of the set of gradients of all
constraint functions, {∇g1(x), . . . , ∇gm(x)}, before writing down the Lagrange conditions
If the set {∇g1(x), . . . , ∇gm(x)} is linearly independent for every x in the constraint set,
then we're completely safe.
If not, things become more complicated, but in simple problems the number of points y in
the constraint set such that {∇g1(y), . . . , ∇gm(y)} is linearly dependent is usually small.
When there are a small number of constraints, we can check what happens when each of
the subsets of the constraints bind (more on that in the next lecture).
ECON 2050  Optimization III
16 / 28
```
