# Norms and sequence limits

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: epsilon-N, convergence, divergence, coordinatewise limits, squeeze.


## Norms and convergence

$$
\|x\|=\sqrt{\sum_i x_i^2},\qquad
\|x-y\|\text{ is the distance from }x\text{ to }y.
$$

$$
x_n\to x^*
\iff
\forall\varepsilon>0\ \exists N\in\mathbb N\ \forall n\ge N:
\|x_n-x^*\|<\varepsilon.
$$

For scalar sequences use $|x_n-x^*|$. Choose $N$ after $\varepsilon$, and make it work for every $n\ge N$. If $|a_n-L|\le C/n$, choose $N>C/\varepsilon$; then $n\ge N$ gives $|a_n-L|<\varepsilon$.

A vector sequence converges exactly when all coordinate sequences converge, with their respective limits as coordinates. Useful estimates are

$$
|x_i-y_i|\le\|x-y\|\le\sum_i|x_i-y_i|,\qquad
\|u+v\|\le\|u\|+\|v\|.
$$

Use the course limit rules for sums, scalar multiples and scalar products/quotients where valid; a quotient needs a nonzero limiting denominator. Bounds such as $|\sin n|\le1$ or $|\cos n|\le1$ can reduce a limit to a vanishing estimate.

To justify divergence, show a violated necessary property, unboundedness, or two subsequences with distinct limits. Oscillation of a factor alone is insufficient: an oscillating term multiplied by a vanishing factor may converge.


## Exact result locators

- [Scalar convergence definition](page-lecture-01-12.md) — Lecture 1, PDF p. 12.
- [Vector convergence and balls](page-lecture-01-18.md) — Lecture 1, PDF p. 18.
- [Coordinatewise convergence](page-lecture-01-25.md) — Lecture 1, PDF p. 25.

## Further source pages

- Lecture 1, PDF pp. [2](page-lecture-01-02.md), [3](page-lecture-01-03.md), [4](page-lecture-01-04.md), [5](page-lecture-01-05.md)
- Lecture 1, PDF pp. [8](page-lecture-01-08.md), [9](page-lecture-01-09.md), [10](page-lecture-01-10.md), [11](page-lecture-01-11.md), [12](page-lecture-01-12.md), [13](page-lecture-01-13.md), [14](page-lecture-01-14.md), [15](page-lecture-01-15.md), [16](page-lecture-01-16.md), [17](page-lecture-01-17.md), [18](page-lecture-01-18.md), [19](page-lecture-01-19.md), [20](page-lecture-01-20.md), [21](page-lecture-01-21.md), [22](page-lecture-01-22.md), [23](page-lecture-01-23.md), [24](page-lecture-01-24.md), [25](page-lecture-01-25.md)
