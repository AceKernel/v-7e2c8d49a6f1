# Lecture 6: Infeasibility-certificate example

PDF page 11 of 26; printed slide 11.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=11) | [Previous](page-lecture-06-10.md) | [Next](page-lecture-06-12.md)

Topics: farkas, graphs.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Example: We use the Farkas lemma to decide the solvability of the system:
⎛
⎜
⎜
⎝
1
1
0
1
0
1
0
1
1
1
1
1
⎞
⎟
⎟
⎠
⎛
⎝
x1
x2
x3
⎞
⎠=
⎛
⎜
⎜
⎝
2
2
2
1
⎞
⎟
⎟
⎠.
We are interested in non-negative solutions of this system. The Farkas alternative is
(︁
y1
y2
y3
y4
)︁
⎛
⎜
⎜
⎝
1
1
0
1
0
1
0
1
1
1
1
1
⎞
⎟
⎟
⎠≥
⎛
⎜
⎜
⎝
0
0
0
0
⎞
⎟
⎟
⎠,
and
2y1 + 2y2 + 2y3 + y4 < 0.
As a system of inequalities the alternative is (ignore the strict inequality for the moment):
⎧
⎪
⎨
⎪
⎩
y1 + y2 + y4 ≥0
y1 + y3 + y4 ≥0
y2 + y3 + y4 ≥0
⇒
⎧
⎪
⎨
⎪
⎩
y1 + y2 ≥−y4
y1 + y3 ≥−y4
y2 + y3 ≥−y4
ECON 2050 – Linear Algebra II
11 / 26
```
