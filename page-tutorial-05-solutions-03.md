# Tutorial 5 solutions: P1: Linear independence and span of vector families; P2: Rank of three matrices; P3: Column-span characterisation of feasibility

PDF page 3 of 5.

[Page map](map-tutorial-05-solutions.md) | [Original PDF page](tutorial-05-solutions.pdf#page=3) | [Previous](page-tutorial-05-solutions-02.md) | [Next](page-tutorial-05-solutions-04.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
