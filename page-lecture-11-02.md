# Lecture 11: Nonnegative decision variables

PDF page 2 of 25; printed slide 2.

[Page map](map-lecture-11.md) | [Original PDF page](lecture-11.pdf#page=2) | [Previous](page-lecture-11-01.md) | [Next](page-lecture-11-03.md)

Topics: kkt.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
A (particularly relevant) special class of problems
In economics, nance, and business, we commonly work with nonnegative variables such as
quantities and prices. Therefore, we often have to solve problems of the form
max
x∈S f (x)
s.t.
g1(x) ≤0, . . . , gm(x) ≤0
(♢)
x1 ≥0, . . . , xn ≥0
(1)
where S ⊆Rn is open and f , g1, . . . , gm : S →R are continuously dierentiable.
Problems of this form are so ubiquitous that, although we can tackle them with our previous
theorem on inequality constraints, a special theorem has been derived for them.
ECON 2050  Optimization IV
2 / 25
```
