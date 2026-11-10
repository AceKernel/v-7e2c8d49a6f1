# Lecture 5: automatic text transcript

Original: [Lecture 5 PDF](lecture-05.pdf). Topic: Span, independence, rank and linear equations.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050 – Mathematical Economics
Linear Algebra I
ECON 2050 – Linear Algebra I
1 / 26
```

## PDF page 2

```text
Vectors
Loosely speaking, a vector is a term that refers to quantities that cannot be expressed by a
single real number.
More specifically, a (m-dimensional) vector is an ordered list of m > 1 real numbers.
To distinguish vectors from scalars (i.e., single numbers), we denote vectors by bold
lowercase letters (e.g., x).
A m-dimensional vector x = (x1, x2, . . . , xn) is an element of Rm.
x1
x2
x = (3, 4)
x1
x2
x = (3, 4)
ECON 2050 – Linear Algebra I
2 / 26
```

## PDF page 3

```text
Scalar multiplication and inner product of vectors
The product of a real number (or scalar) c ∈R and an (m-dimensional) vector
x = (x1, x2, . . . , xm) ∈Rm, denoted by cx, is given by
cx = (cx1, cx2, . . . , cxm).
Also recall that in Lecture 2, we defined the inner product (or dot product) of two
(m-dimensional) vectors x, y ∈Rm by
x · y =
m
∑︂
i=1
xiyi = x1y1 + x2y2 + . . . + xmym.
ECON 2050 – Linear Algebra I
3 / 26
```

## PDF page 4

```text
Linear combination
Let S = {x1, x2, . . . , xn} be a set of vectors (say in Rm).
A vector y can be expressed as a linear combination of vectors in S = {x1, x2, . . . , xn} if
there are real numbers a1, a2, . . . , an such that
y =
n
∑︂
j=1
aj xj.
The set of all vectors that can be expressed as a linear combination of vectors in S is called
the span of S and denoted span(S).
ECON 2050 – Linear Algebra I
4 / 26
```

## PDF page 5

```text
Example: Consider the set of vectors S = {(0, 1), (2, 1)}.
span(S) is the set of all linear combinations of the vectors in S. Since S contains two vectors
x1 = (0, 1) and x2 = (2, 1), the span is
span(S) = {a1(0, 1) + a2(2, 1) : a1, a2 ∈R}
= {(0 · a1 + 2 · a2, 1 · a1 + 1 · a2) : a1, a2 ∈R}
= {(2a2, a1 + a2) : a1, a2 ∈R}
But then any vector x = (x1, x2) ∈R2 can be written as (2a2, a1 + a2) by letting a2 = x1/2
and a1 = x2 −x1/2. Thus, span(S) = R2.
ECON 2050 – Linear Algebra I
5 / 26
```

## PDF page 6

```text
Linear independence and dependence
The set S of vectors is said to be linearly independent if
n
∑︂
j=1
aj xj = 0
implies
aj = 0 for all j = 1, . . . , n,
where 0 denotes the zero vector (0, 0, . . . , 0). And the set S is said to be linearly dependent
if it is not linearly independent; that is, there exist a1, a2, . . . , an ∈R, not all zero, such that
n
∑︂
j=1
aj xj = 0.
In words, a set of vectors is linearly dependent if at least one of its elements can be expressed
as a linear combination of some other elements; and a set of vectors is linearly independent if
none of its elements can be expressed as a linear combination of some other elements.
ECON 2050 – Linear Algebra I
6 / 26
```

## PDF page 7

```text
Example: Any set of vectors that contains only one vector that is not 0 is (trivially) linearly
independent.
For example, the set T = {(1, −2)} is linearly independent.
But the set O = {(0, 0)} is linearly dependent.
Example: Consider, once again, the set of vectors S = {(0, 1), (2, 1)}. To see whether it is
linearly independent, consider
a1(0, 1) + a2(2, 1) = (0, 0).
This can be written as (2a2, a1 + a2) = (0, 0), which requires 2a2 = 0 and a1 + a2 = 0. From
the first equation, we know that a2 = 0; plugging it back into the second equation, we see
that a1 = 0. Therefore, S must be linearly independent.
ECON 2050 – Linear Algebra I
7 / 26
```

## PDF page 8

```text
Example: Straightforwardly, the set of vectors R = {(1, −2), (2, −4)} is linearly dependent.
This is because
2(1, −2) = (2, −4)
⇐⇒
2(1, −2) −(2, −4) = (0, 0).
That is, there exist a1 = 2 and a2 = −1 (both nonzero) such that
a1(1, −2) + a2(2, −4) = (0, 0).
Example: Consider the set of vectors P = {(1, 1, 0), (0, −3, 1), (2, 5, −1)}. This set is also
linearly dependent because
(2, 5, −1) = 2(1, 1, 0) −(0, −3, 1)
⇐⇒
2(1, 1, 0) −(0, −3, 1) −(2, 5, −1) = (0, 0, 0).
ECON 2050 – Linear Algebra I
8 / 26
```

## PDF page 9

```text
x1
x2
O
(2, −4)
(1, −2)
1
2
3
4
-1
-2
-3
-4
x1
x2
O
(0, 1)
(2, 1)
1
2
3
4
1
2
3
4
The linearly dependent vectors (1, −2) and (2, −4) are “collinear” in the sense that they
lie on the same line through the origin.
The linearly independent vectors (0, 1) and (2, 1) are not collinear, which suffices for
spanning the entire plane (R2).
ECON 2050 – Linear Algebra I
9 / 26
```

## PDF page 10

```text
Rank
The rank of a set S of vectors is the maximal number of linearly independent vectors in S,
denoted by rank(S).
If S is a set of vectors in Rm, then the discussion on the previous slide indicates that
rank(S) ≤m.
Examples:
T = {(1, −2)}, rank = 1;
S = {(0, 1), (2, 1)}, rank = 2;
B = {(0, 1), (1, 0)}, rank = 2;
R = {(1, −2), (2, −4)}, rank = 1;
P = {(1, 1, 0), (0, −3, 1), (2, 5, −1)}, rank = 2.
ECON 2050 – Linear Algebra I
10 / 26
```

## PDF page 11

```text
From vectors to matrices
Consider a vector x = (1, 2, 3). It can be written either as a “row array of numbers,”
x = (1
2
3), or as a “column array of numbers:”
x =
⎛
⎝
1
2
3
⎞
⎠.
Consequently, a set of vectors in Rm can be interpreted in the following way: either take each
element as a row array, or take each element as a column array, and then “stack” them
together. For example, if S = {(1, 2, 3), (4, 5, 6)}, then by interpreting each element as a row
array and a column array, we get, respectively, matrices
(︃1
2
3
4
5
6
)︃
and
⎛
⎝
1
4
2
5
3
6
⎞
⎠.
Conversely, it will be useful later on to think of the columns and rows of a matrix as vectors.
ECON 2050 – Linear Algebra I
11 / 26
```

## PDF page 12

```text
Matrices: Basics
A rectangular array of numbers consisting of m rows and n columns is called an m × n matrix.
A matrix is usually denoted by a bold uppercase letter (e.g., A), and the number in the
i-th row and j-th column is denoted aij.
Whenever we use lowercase letters to denote the numbers appearing in the matrix, we use
the corresponding bold uppercase letters to denote the matrix.
For a matrix A, the i-th row is denoted ai and the j-th column is denoted aj.
If A is a matrix, its transpose, written A⊺is the matrix obtained by interchanging the
columns of A with its rows.
Example: If the matrix
A =
(︃0
1
2
1
)︃
then
A⊺=
(︃0
2
1
1
)︃
.
ECON 2050 – Linear Algebra I
12 / 26
```

## PDF page 13

```text
For a vector x ∈Rm,
when interpreted as a row array it is equivalent to a 1 × m matrix; and
when interpreted as a column array it is equivalent to a m × 1 matrix.
Thus, when we wish to emphasize the interpretation we adopt, we will call x either a “1 × m
vector” or a “m × 1 vector.”
Defining the product of a matrix and a vector will be useful:
The product of an m × n matrix A with a n × 1 vector x = (x1, . . . , xn), Ax, is the m × 1
vector whose i th component is ∑︁n
j=1 aijxj.
The i th component can also be written using inner product (dot product) notation as
ai · x.
The product of an 1 × m vector y = (y1, . . . , ym) and a m × n matrix A, yA, is the 1 × n
vector whose j th component is ∑︁m
i=1 aijyi.
The j th component can also be written using inner product (dot product) notation as
y · aj.
ECON 2050 – Linear Algebra I
13 / 26
```

## PDF page 14

```text
The column rank of a matrix is the maximal number of its linearly independent columns.
Similarly, the row rank is the maximal number of its linearly independent rows.
Consider an m × n matrix A. It can either be represented by its rows:
A =
⎛
⎜
⎜
⎜
⎝
a1
a2
...
am
⎞
⎟
⎟
⎟
⎠,
or by its columns: A =
(︁
a1
a2
· · ·
an)︁
. Then the row rank of A is the rank of the set of
vectors AR = {a1, a2, . . . , am}, and the column rank of A is the rank of the set of vectors
AC = {a1, a2, . . . , an}.
ECON 2050 – Linear Algebra I
14 / 26
```

## PDF page 15

```text
Theorem
Let A be an m × n matrix. Then its column rank and row rank coincide.
The formal proof of this result is beyond the scope of this course, but it makes intuitive sense:
Let’s revisit the example of the set of vectors S = {(1, 2, 3), (4, 5, 6)}.
If we interpret each vector in S as a row, we get a matrix
A =
(︃1
2
3
4
5
6
)︃
.
Interpreting each vector in S as a column, we get a matrix
B =
⎛
⎝
1
4
2
5
3
6
⎞
⎠= A⊺.
But the rank of a set of vectors shouldn’t be affected by the way we interpret the vectors.
ECON 2050 – Linear Algebra I
15 / 26
```

## PDF page 16

```text
Therefore, we define the rank of a matrix to be its column rank (or row rank, which is the
same).
We denote the rank of a matrix A by rank(A).
Our discussion on the the previous two slides together imply the following result:
Corollary
Let A be an m × n matrix. Then rank(A) ≤min{m, n}.
Finally, if A is a matrix we will write span(A) to denote the span of the columns of A.
For example, if the columns of matrix A are vectors a1, a2, a3, and let AC = {a1, a2, a3}.
Then span(A) = span(AC).
ECON 2050 – Linear Algebra I
16 / 26
```

## PDF page 17

```text
Let A be an m × n matrix.
We can augment a (m × 1) vector b to its right, and denote the augmented matrix by
[A|b].
We can also augment a m × k matrix C to its right; denote the augmented matrix by
[A|C].
Example: Consider
A =
⎛
⎝
0
1
2
1
4
0
⎞
⎠,
b =
⎛
⎝
3
5
2
⎞
⎠,
and
C =
⎛
⎝
0
1
0
−2
2
0
−2
3
0
⎞
⎠.
Then
[A|b] =
⎛
⎝
0
1
3
2
1
5
4
0
2
⎞
⎠,
and
[A|C] =
⎛
⎝
0
1
0
1
0
2
1
−2
2
0
4
0
−2
3
0
⎞
⎠.
ECON 2050 – Linear Algebra I
17 / 26
```

## PDF page 18

```text
Historically, matrices are introduced in the study of solving linear equations.
For example, the system of equations
{︄
−4x1 + 2x2 −5x3
= 1
2x1 −x2 + 2.5x3
= 1
can be written as Ax = b, where
A =
(︃−4
2
−5
2
−1
2.5
)︃
,
x =
⎛
⎝
x1
x2
x3
⎞
⎠,
and
b =
(︃1
1
)︃
.
ECON 2050 – Linear Algebra I
18 / 26
```

## PDF page 19

```text
Feasibility
We will be interested in problems of the following kind:
Given an m × n matrix A and b ∈Rm, find an x ∈Rn such that Ax = b or prove that
no such x exists.
These problems are ultimately about whether a system of linear equations has a solution.
The problem of whether we can find an x ∈Rn such that Ax = b can be stated as: is
b ∈span(A)?
Convincing another that the system has a solution (when it does) is easy: just verify.
However, convincing another that it doesn’t have a solution can be much more difficult:
there are infinitely many possibilities.
ECON 2050 – Linear Algebra I
19 / 26
```

## PDF page 20

```text
Consider the system of equations
(︃−4
2
−5
2
−1
2.5
)︃⎛
⎝
x1
x2
x3
⎞
⎠=
(︃1
1
)︃
,
and suppose we wish to know if it has a solution.
For the moment suppose that it does, and denote it by x∗. Then
Adding a linear multiple of one equation to the other yields another equation that x∗
must also satisfy.
We multiply the second equation by 2 and add it to the first.
This produces 0x1 + 0x2 + 0x3 = 3, which cannot admit a solution.
This suggests that we might be able to decide the insolvability of a system by deriving,
through appropriate linear combinations of the given equations, an inconsistency.
ECON 2050 – Linear Algebra I
20 / 26
```

## PDF page 21

```text
Solvability of linear equations
Theorem
Let A be an m × n matrix, b ∈Rm, and F = {x ∈Rn : Ax = b}. Then either F ̸= ∅or there
exists y ∈Rm such that yA = 0 and y · b ̸= 0 but not both.
In words: Consider a system of m linear equations with n unknowns. Then either the system
of linear equations has a solution, or we can find m “weights,” one on each of the equations,
that derives an inconsistency.
ECON 2050 – Linear Algebra I
21 / 26
```

## PDF page 22

```text
Geometric interpretation:
Suppose F = ∅. Then, b is not in the span of the columns of A.
If we think of the span of the columns of A as a plane, then b is a vector pointing out of
the plane.
Thus, any vector, y, orthogonal to this plane (and so to every column of A) must have a
non-zero inner product (dot product) with b.
ECON 2050 – Linear Algebra I
22 / 26
```

## PDF page 23

```text
Algebraic intuition:
Take any linear combination of the equations in the system Ax = b.
This linear combination can be obtained by multiplying each side of the system by a
suitable vector y: yAx = y · b.
Any vector that solves the first system must also solve the second.
If yA = 0, then yAx = 0 · x = 0 for any x ∈Rn. But then y · b ̸= 0 implies that
yAx ̸= y · b.
Thus, there doesn’t exists a vector x such that yAx ̸= y · b, which in turn implies that
Ax = b is impossible.
ECON 2050 – Linear Algebra I
23 / 26
```

## PDF page 24

```text
Example: Consider, once again, the system of linear equations Ax = b, where
A =
(︃−4
2
−5
2
−1
2.5
)︃
,
x =
⎛
⎝
x1
x2
x3
⎞
⎠,
and
b =
(︃1
1
)︃
.
Consider a vector y = (y1, y2), and suppose
yA =
(︁
y1
y2
)︁(︃−4
2
−5
2
−1
2.5
)︃
=
(︁
−4y1 + 2y2
2y1 −y2
−5y1 + 2.5y2
)︁
= 0;
this is equivalent to 2y1 = y2. But y · b = y1 + y2; if y1 = 1 and y2 = 2, we have yA = 0 but
y · b = 3 ̸= 0, and therefore it must be that the system of equations has no solution.
ECON 2050 – Linear Algebra I
24 / 26
```

## PDF page 25

```text
Sometimes the solvability of a system of linear equations is more conveniently determined by
the following result (will not appear in any assignments or exam):
Theorem
Let A be an m × n matrix of rank r and b ∈Rm. Let r′ be the rank of the augmented matrix
[A | b] and let F = {x ∈Rn : Ax = b}. Then exactly one of the following must be true:
(i) if r′ = r + 1, F = ∅;
(ii) if r′ = r = n, F is a single vector;
(iii) if r = r′ < n, then F contains infinitely many vectors.
r′ = r + 1 implies that b cannot be written as a linear combination of columns of A; i.e.,
b /∈span(A). This means that there doesn’t exist x ∈Rn such that Ax = b, and hence
the system has no solution.
r′ = r means that b can be written as a linear combination of columns of A:
b ∈span(A). Thus, a solution exists. If r = n, there are n equations and n unknowns,
and therefore exactly one solution; if r < n, some equations are “redundant.”
ECON 2050 – Linear Algebra I
25 / 26
```

## PDF page 26

```text
Example: Consider, yet another time, the system of linear equations Ax = b, where
A =
(︃−4
2
−5
2
−1
2.5
)︃
,
x =
⎛
⎝
x1
x2
x3
⎞
⎠,
and
b =
(︃1
1
)︃
.
Observe that
[A | b] =
(︃−4
2
−5
1
2
−1
2.5
1
)︃
.
It can be verified that rank(A) = 1, and rank([A | b]) = 2. Then by the theorem on the
previous slide, the system of equations has no solution.
Example: Consider another system of linear equations Ax = c, where A and x are identical to
the previous example, and c =
(︃1
−2
)︃
. Now rank([A | c]) = 1, and therefore the system has
infinitely many solutions.
ECON 2050 – Linear Algebra I
26 / 26
```
