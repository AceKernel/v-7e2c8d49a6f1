# Tutorial 6, Problem 2: A Farkas feasibility certificate

[Problem index](QUESTIONS.md) | [Page map](map-tutorial-06-solutions.md) | [Original PDF](tutorial-06-solutions.pdf)

Topics: farkas.

> Unverified automatic extraction of the supplied official question and solution, not a checked LaTeX transcription. Fractions, exponents, symbols and diagrams may be corrupted; check the linked original pages. Source wording and any source errors are retained.

## PDF page 2

[Original page](tutorial-06-solutions.pdf#page=2)

```text
Problem 2
Use the Farkas lemma to decide if the following system has a non-negative solution:

4
1
−5
1
0
2
 

x1
x2
x3

=

1
1

.
Solution: The Farkas alternative is
y1
y2
 
4
1
−5
1
0
2

≥
0
0
0
,
and
y1 + y2 < 0.
As a system of inequalities the alternative is:
4y1 + y2 ≥0,
y1 + 0y2 ≥0,
−5y1 + 2y2 ≥0,
y1 + y2 < 0.
There can be no solution to this system. The second inequality requires that y1 ≥0. Combin-
ing this with the last inequality we conclude that y2 < 0. But y1 ≥0 and y2 < 0 contradict
−5y1 + 2y2 ≥0. Thus, the original system has a non-negative solution.
```
