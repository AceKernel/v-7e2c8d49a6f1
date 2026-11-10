# Lecture 10: Binding and slack pairs

PDF page 4 of 28; printed slide 4.

[Page map](map-lecture-10.md) | [Original PDF page](lecture-10.pdf#page=4) | [Previous](page-lecture-10-03.md) | [Next](page-lecture-10-05.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Consequently, we can treat every primal constraint and its corresponding dual variable as a
complementary pair: if one is slack the other one must be binding. Thus,
y∗
i
⎛
⎝
n
∑︂
j=1
aijx∗
j −bi
⎞
⎠= 0
for every i = 1, . . . , m.
(CS1)
Similarly, we can treat every dual constraint and its corresponding primal variable as a
complementary pair: if one is slack the other one must be binding. Thus,
x∗
j
(︄m
∑︂
i=1
aijy∗
i −cj
)︄
= 0
for every j = 1, . . . , n.
(CS2)
The conditions (CS1) and (CS2) are called the complementary slackness conditions.
As we will soon see, these conditions can be very useful in solving linear or even non-linear
programming problems.
ECON 2050  Optimization III
4 / 28
```
