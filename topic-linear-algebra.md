# Span, independence and linear systems

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: rank, row rank, column rank, feasibility, unrestricted certificates.


## Span, independence and rank

$$
\operatorname{span}\{v^1,\ldots,v^k\}
=\left\{\sum_{j=1}^k a_jv^j:a_j\in\mathbb R\right\}.
$$

The vectors are linearly independent if $\sum_j a_jv^j=0$ implies every $a_j=0$. To prove dependence, exhibit coefficients not all zero with zero combination. Rank is the largest number of linearly independent vectors; matrix row rank and column rank coincide.

For $A\in\mathbb R^{m\times n}$, its columns lie in $\mathbb R^m$ and $x\in\mathbb R^n$. The system $Ax=b$ is feasible exactly when $b$ belongs to the span of the columns. Show a solution or derive an inconsistency; distinguish free coefficients from nonnegative ones.

## Unrestricted-system alternative

Exactly one of the following holds:

$$
\exists x\in\mathbb R^n:\ Ax=b,
\qquad\text{or}\qquad
\exists y\in\mathbb R^m:\ yA=0,\quad y\cdot b\ne0.
$$

The course writes $y$ as a row multiplier. For a proposed infeasibility certificate, compute $yA$ and $y\cdot b$ explicitly. If both a solution and certificate existed, $y\cdot b=yAx=0$, a contradiction.

For nonnegative coefficients use [cones and Farkas](topic-farkas.md), not this unrestricted alternative. Lecture 5 PDF page 25 explicitly says its separate augmented-rank solvability criterion will not appear in assignments/exam; that source is retained for completeness. This does not exclude the course's other rank, span and independence questions.


## Exact result locators

- [Span](page-lecture-05-04.md) — Lecture 5, PDF p. 4.
- [Linear independence](page-lecture-05-06.md) — Lecture 5, PDF p. 6.
- [Row rank equals column rank](page-lecture-05-15.md) — Lecture 5, PDF p. 15.
- [Unrestricted-system alternative](page-lecture-05-21.md) — Lecture 5, PDF p. 21.
- [Explicitly excluded rank criterion](page-lecture-05-25.md) — Lecture 5, PDF p. 25.

## Further source pages

- Lecture 5, PDF pp. [2](page-lecture-05-02.md), [3](page-lecture-05-03.md), [4](page-lecture-05-04.md), [5](page-lecture-05-05.md), [6](page-lecture-05-06.md), [7](page-lecture-05-07.md), [8](page-lecture-05-08.md), [9](page-lecture-05-09.md), [10](page-lecture-05-10.md), [11](page-lecture-05-11.md), [12](page-lecture-05-12.md), [13](page-lecture-05-13.md), [14](page-lecture-05-14.md), [15](page-lecture-05-15.md), [16](page-lecture-05-16.md), [17](page-lecture-05-17.md), [18](page-lecture-05-18.md), [19](page-lecture-05-19.md), [20](page-lecture-05-20.md), [21](page-lecture-05-21.md), [22](page-lecture-05-22.md), [23](page-lecture-05-23.md), [24](page-lecture-05-24.md), [25](page-lecture-05-25.md), [26](page-lecture-05-26.md)
- Lecture 6, PDF pp. [2](page-lecture-06-02.md), [3](page-lecture-06-03.md)
- Annotated revision lecture, PDF pp. [19](page-revision-lecture-19.md)

## Official worked problems

- [Tutorial 5, Problem 1: Linear independence and span of vector families](problem-tutorial-05-01.md)
- [Tutorial 5, Problem 2: Rank of three matrices](problem-tutorial-05-02.md)
- [Tutorial 5, Problem 3: Column-span characterisation of feasibility](problem-tutorial-05-03.md)
- [Tutorial 5, Problem 4: Linear-system feasibility and certificates](problem-tutorial-05-04.md)
