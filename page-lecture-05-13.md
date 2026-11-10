# Lecture 5: Matrix dimensions

PDF page 13 of 26; printed slide 13.

[Page map](map-lecture-05.md) | [Original PDF page](lecture-05.pdf#page=13) | [Previous](page-lecture-05-12.md) | [Next](page-lecture-05-14.md)

Topics: linear-algebra.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
