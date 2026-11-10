# Tutorial 5 solutions: P3: Column-span characterisation of feasibility; P4: Linear-system feasibility and certificates

PDF page 4 of 5.

[Page map](map-tutorial-05-solutions.md) | [Original PDF page](tutorial-05-solutions.pdf#page=4) | [Previous](page-tutorial-05-solutions-03.md) | [Next](page-tutorial-05-solutions-05.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
Problem 4
Consider the system of equations

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

.
4
```
