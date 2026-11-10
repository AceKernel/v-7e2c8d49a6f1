# Tutorial 5, Problem 3: Column-span characterisation of feasibility

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-05-solutions.md) | [Original PDF](tutorial-05-solutions.pdf)

Topics: linear-algebra.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 3

[Original page](tutorial-05-solutions.pdf#page=3)

```text
Problem 3
Let A be a m×n matrix, and b ∈Rm. In the lecture we claimed that “there exists x ∈Rn
such that Ax = b” is equivalent to “b ∈span(A).” Carefully argue why this assertion is
true, and offer an example where m = 2 and n = 3.
Solution: First, let’s analyze the statement “there exists x ∈Rn such that Ax = b.” Let A
be an m × n matrix. We can represent it by its columns: A =
a1
a2
· · ·
an
, where
3
```

## PDF page 4

[Original page](tutorial-05-solutions.pdf#page=4)

```text
ECON 2050
S2 2026
each column ai is a vector in Rm. Let x be a (n × 1) vector in Rn:
x =




x1
x2...
xn



.
By the definition of matrix-vector multiplication, the product Ax is a linear combination of
the columns of A using the components of x as weights (or coefficients):
Ax = x1a1 + x2a2 + · · · + xnan.
Therefore, the equation Ax = b is just a compact way of writing
x1a1 + x2a2 + · · · + xnan = b,
implying that b can be written as a linear combination of the columns of A.
Now let’s turn to the statement “b ∈span(A).” Recall that span(A) is defined as the
span of the set of column vectors of A, which we can write as AC := {a1, a2, . . . , an}.
By definition, this means that b can be expressed as a linear combination of vectors in AC,
or the columns of A. But this is precisely the meaning of “there exists x ∈Rn such that
Ax = b.” The equivalence thus follows.
For the example, we can let
A =

4
1
−2
1
0
5

and
b =

−2
3

.
Then “there exists x ∈Rn such that Ax = b” means that

4
1
−2
1
0
5
 

x1
x2
x3

=

−2
3

,
or equivalently
x1

4
1

+ x2

1
0

+ x3

−2
5

=

−2
3

.
And “b ∈span(A)” means that b is in the span of the set of columns {(4, 1), (1, 0), (−2, 5)}.
That is, b can be written as a linear combination of the columns of A:
x1

4
1

+ x2

1
0

+ x3

−2
5

=

−2
3

.
```
