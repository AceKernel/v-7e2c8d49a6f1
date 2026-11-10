# Lecture 6: Constructing a certificate

PDF page 12 of 26; printed slide 12.

[Page map](map-lecture-06.md) | [Original PDF page](lecture-06.pdf#page=12) | [Previous](page-lecture-06-11.md) | [Next](page-lecture-06-13.md)

Topics: farkas, graphs.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
To maximize the chance of satisfying the strict inequality 2y1 + 2y2 + 2y3 + y4 < 0, we let
y1, y2, y3 to be “as negative as they can” (i.e., without violating the other three inequalities):
To that end, we let all three inequalities on the previous slide hold with equality; adding
them together yields 2y1 + 2y2 + 2y3 = −3y4.
Consequently, it must be that 2y1 + 2y2 + 2y3 + y4 < 0, implying that the alternative
must have a solution. In particular, one solution is y1 = y2 = y3 = −1, and y4 = 2.
By the Farkas lemma, the original system has no solution.
In a vague sense, the solution to the alternative we identify provides an “explanation” for why
the (original) system has no solution:
Multiply the first three equations by −1 and add them together to yield
−2x1 −2x2 −2x3 = −6.
However, this is inconsistent with the fourth equation multiplied by 2:
2x1 + 2x2 + 2x3 = 2.
ECON 2050 – Linear Algebra II
12 / 26
```
