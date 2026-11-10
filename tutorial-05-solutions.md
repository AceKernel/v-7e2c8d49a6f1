# Tutorial 5 solutions: automatic text transcript

Original: [Tutorial 5 solutions PDF](tutorial-05-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050
S2 2026
Tutorial 5 Solution
Problem 1
Consider the following sets of vectors. Determine (a) whether they are linear indepen-
dent or linearly dependent, and (b) their spans.
(i) S1 = {(1, −2), (2, −4)};
(ii) S2 = {(1, 0), (0, 1)};
(iii) S3 = {(0, 1, 0), (−2, 2, 0)};
(iv) S4 = {(0, 1, 0), (−2, 2, 0), (−2, 3, 0)};
(v) S5 = {(1, 1, 0), (0, −3, 1), (2, 4, −1)}.
Solution:
(i) We know from lecture slides that S1 is linearly dependent; and
span(S1) = {a1(1, −2) + a2(2, −4) : a1, a2 ∈R} .
Since (2, −4) = 2(1, −2), we can simplify it to
span(S1) = {a1(1, −2) + 2a2(1, −2) : a1, a2 ∈R} = {(a1 + 2a2)(1, −2) : a1, a2 ∈R} .
If we let k = c1 +2c2, we can see that any vector in the span is just a scalar multiple of
(1, −2). This is precisely the line that passes through the origin and the point (1, −2).
In other words, the span is the set of all points (x, y) that satisfy the equation y = −2x.
(ii) To see that whether S2 is linearly independent, consider
a1(1, 0) + a2(0, 1) = (0, 0).
This is equivalent to a1 = 0 and a2 = 0, and therefore S2 must be linearly independent.
And its span is given by
span(S2) = {a1(1, 0) + a2(0, 1) : a1, a2 ∈R} = {(a1, a2) : a1, a2 ∈R} = R2.
(iii) Again, we consider the equality
a1(0, 1, 0) + a2(−2, 2, 0) = (0, 0, 0).
Since the left-hand side is equivalent to (−2a2, a1+2a2, 0), the equality above is equiv-
alent to −2a2 = 0 and a1 + 2a2 = 0. Then it must be that a1 = a2 = 0, showing that
S3 is linearly independent.
1
```

## PDF page 2

```text
ECON 2050
S2 2026
For its span,
span(S3) = {a1(0, 1, 0) + a2(−2, 2, 0) : a1, a2 ∈R} = {(−2a2, a1 + 2a2, 0) : a1, a2 ∈R} .
Note that no matter what a1 and a2 we choose, the third entry is always zero. And
any vector (x, y, 0) ∈R2 can be written as (−2a2, a1 + 2a2) by letting a2 = −x/2 and
a1 = y + x. Thus,
span(S3) = {(x, y, 0) : x, y ∈R}.
Geometrically, the set of all vectors where the z-component is zero forms a flat, two-
dimensional plane, sometimes called the xy-plane.
(iv) S4 is linearly dependent because (−2, 3, 0) = (0, 1, 0) + (−2, 2, 0), or equivalently,
(−2, 3, 0) −(0, 1, 0) −(−2, 2, 0) = (0, 0, 0).
By comparing S3 in part (iii) and S4, we see that S4 = S3 ∪{(−2, 3, 0)}. But since the
vector (−2, 3, 0) can be written as a linear combination of elements in S3, it belongs to
the span of S3, and therefore including this vector doesn’t enlarge the span. Therefore,
span(S4) = span(S3) = {(x, y, 0) : x, y ∈R}.
(v) To determine whether S5 is linearly independent, we consider
a1(1, 1, 0) + a2(0, −3, 1) + a3(2, 4, −1) = (0, 0, 0).
This is equivalent to
a1 + 2a3 = 0
a1 −3a2 + 4a3 = 0
a2 −a3 = 0
We see from the last equation that a2 = a3; plugging it to the second equation, we get
a1 + a3 = 0. Now compare it with the first equation, we get a3 = 0. Then because
a2 = a3 and a1 + a3 = 0, it must be that a1 = a2 = a3 = 0, showing that S5 is linearly
independent.
It is routine to see that
span(S5) = {a1(1, 1, 0) + a2(0, −3, 1) + a3(2, 4, −1) : a1, a2, a3 ∈R}
= {(a1 + 2a3, a1 −3a2 + 4a3, a2 −a3) : a1, a2, a3 ∈R}.
One can verify that every vector (x1, x2, x3) ∈R3 can be written as (a1 + 2a3, a1 −
3a2 + 4a3, a2 −a3) by solving the system of equations
a1 + 2a3 = x1
a1 −3a2 + 4a3 = x2
a2 −a3 = x3
and getting
a1 = −x1 + 2x2 + 6x3
a2 = x1 −x2 −2x3
a2 = x1 −x2 −3x3
Thus, span(S5) = R3.
2
```

## PDF page 3

```text
ECON 2050
S2 2026
Problem 2
Determine the rank of the following matrices:
A =


1
0
2
1
−3
4
0
1
−1

,
B =


0
1
0
−2
2
0
−2
3
0

,
and
C =


2
0
−1
3
1
1
2
2
2
0
−1
1

.
Solution: We consider the matrix A first. To calculate its rank, we need to find the rank of its
columns (or, equivalently, the maximal number of its linearly independent columns), which
is just rank(S5). Then because we showed in Problem 1 part (v) that in S5, the maximal
number of linearly independent vectors is three, we conclude that rankA = rank(S5) = 3.
For the matrix B, note that its rank also equals to the rank of its rows (or, equivalently,
the maximal number of its linearly independent rows), which is just rank(S4). Then because
we showed in Problem 1 part (iv) that in S4, the maximal number of linearly independent
vectors is two, we conclude that rankA = rank(S4) = 2.
Finally, for the matrix C, rankC equals to the rank of its rows, namely the rank of
the set CR ≡{c1, c2, c3}, where c1 =
2
0
−1
3
, c2 =
1
1
2
2
, and c3 =
2
0
−1
1
. To understand the number of maximal linearly independent vectors in CR,
consider the equation a1c1 + a2c2 + a3c3 = 0, which is equivalent to the following four
equations:
2a1 + a2 + 2a3 = 0
a2 = 0
−a1 + 2a2 −a3 = 0
3a1 + 2a2 + a3 = 0
Plugging c2 = 0 into the other three equations, we get
a1 = −a3
3a1 = −a3
then plug the first equation to the second, we obtain −3a3 = −a3, and therefore −2a3 = 0,
implying that a3 = 0. Then because a1 = −a3, a1 = 0. Thus, a1 = a2 = a3 = 0,
which means that CR is linearly independent. Namely, the maximal number of linearly
independent vectors in CR is 3. Thus, rankC = rank(CR) = 3.
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

## PDF page 5

```text
ECON 2050
S2 2026
(1) Determine whether the system has a solution.
(2) (Extra Practice Problem) Determine whether the system has a solution, and if a
solution exists, whether it has one or infinitely many solutions.
Solution:
(1) Take any vector y = (y1, y2), and let
yA =
y1
y2
 
4
1
−2
1
0
5

=
4y1 + y2
y1
−2y1 + 5y2

=
0
0
0
.
Then it must be that y1 = 0, and plugging this into 4y1 + y2 = 0, we have y2 = 0.
Consequently, y · b = 0 · −2 + 0 · 3 = 0. Thus, whenever yA = 0, it must be that
y · b = 0. The theorem on the slides then indicates that the system has a solution.
(2) We have
[A|b] =

4
1
−2
−2
1
0
5
3

;
it is routine to verify that rank(A) = rank([A|b]) = 2 < 3 = n, and therefore by the
theorem on the slides, the system of equations has infinitely many solutions.
5
```
