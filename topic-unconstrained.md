# Unconstrained optimisation

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: local/global extrema, critical points, saddle points, transformations, boundary comparison.


## Extrema and first-order conditions

A global maximiser has $f(x^*)\ge f(x)$ for every feasible $x$. A local maximiser requires this only in a sufficiently small feasible neighbourhood. Reverse the inequalities for minima.

At an interior local extremum of a differentiable function on an open domain,

$$
\nabla f(x^*)=0.
$$

This condition is necessary, not sufficient: critical points can be maxima, minima or neither. Do not impose it on a boundary optimum as if the point were interior.

## Global sufficiency and transformations

On an open convex domain, a critical point of a differentiable concave function is a global maximiser; for a convex function it is a global minimiser. Strict concavity/convexity gives at most one corresponding global optimizer. It does not by itself ensure an optimizer exists.

For a twice continuously differentiable one-variable function near a critical point, $f''(x^*)<0$ gives a strict local maximum and $f''(x^*)>0$ a strict local minimum. A zero second derivative is inconclusive.

$$
\arg\min_D f=\arg\max_D(-f).
$$

A strictly increasing transformation preserves the maximizing and minimizing points on the valid domain, but changes objective values. If $\ln u$ is replaced by $u$, retain the original restriction $u>0$.

For a compact feasible set, first establish existence, then examine interior critical points and every relevant boundary piece/corner. Check feasibility and domain and compare objective values. For a quadratic, completing squares can prove curvature or give a direct global bound in the course style.


## Exact result locators

- [Local and global extrema](page-lecture-08-04.md) — Lecture 8, PDF p. 4.
- [Interior first-order necessity](page-lecture-08-06.md) — Lecture 8, PDF p. 6.
- [Concavity and global sufficiency](page-lecture-08-12.md) — Lecture 8, PDF p. 12.
- [Increasing transformations](page-lecture-08-19.md) — Lecture 8, PDF p. 19.
- [Interior and boundary candidate procedure](page-lecture-08-23.md) — Lecture 8, PDF p. 23.

## Further source pages

- Lecture 8, PDF pp. [2](page-lecture-08-02.md), [3](page-lecture-08-03.md), [4](page-lecture-08-04.md), [5](page-lecture-08-05.md), [6](page-lecture-08-06.md), [7](page-lecture-08-07.md), [8](page-lecture-08-08.md), [9](page-lecture-08-09.md), [10](page-lecture-08-10.md), [11](page-lecture-08-11.md), [12](page-lecture-08-12.md), [13](page-lecture-08-13.md), [14](page-lecture-08-14.md), [15](page-lecture-08-15.md), [16](page-lecture-08-16.md), [17](page-lecture-08-17.md), [18](page-lecture-08-18.md), [19](page-lecture-08-19.md), [20](page-lecture-08-20.md), [21](page-lecture-08-21.md), [22](page-lecture-08-22.md), [23](page-lecture-08-23.md), [24](page-lecture-08-24.md), [25](page-lecture-08-25.md)
- Annotated revision lecture, PDF pp. [18](page-revision-lecture-18.md)

## Official worked problems

- [Tutorial 8, Problem 1: Affine-inner composition, quadratic curvature and extrema](problem-tutorial-08-01.md)
- [Tutorial 8, Problem 2: Logarithmic domain and absence of extrema](problem-tutorial-08-02.md)
- [Tutorial 8, Problem 4: Quadratic profit and a global maximum](problem-tutorial-08-04.md)
- [Tutorial 9, Problem 1: Graphical optimisation on different feasible sets](problem-tutorial-09-01.md)
- [Tutorial 11, Problem 2: Cobb-Douglas choice and an increasing transformation](problem-tutorial-11-02.md)
