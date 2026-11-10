# Existence of an optimum

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: extreme value theorem, Weierstrass, nonempty compact feasible set.


## Extreme value theorem

A continuous real-valued function on a nonempty compact set $D\subseteq\mathbb R^n$ attains a global maximum and a global minimum. In Euclidean space, compact means closed and bounded.

An existence proof should establish:

1. **Nonempty:** exhibit one feasible point.
2. **Closed:** justify inclusion of boundary points, an intersection of closed sets, or an appropriate limit/ball argument.
3. **Bounded:** exhibit $M$ such that $\|x\|\le M$ for every $x\in D$.
4. **Continuous objective:** name the valid continuity results and check domains.
5. Apply the theorem to conclude attainment, not merely a finite supremum/infimum.

For example, if $D=\{(x,y):|x|+|y|\le2\}$, then $(0,0)\in D$ and

$$
\sqrt{x^2+y^2}\le |x|+|y|\le2.
$$

The set is closed because $(x,y)\mapsto |x|+|y|$ is continuous and the inequality is non-strict; a direct exterior-ball proof is also valid. The norm objective is continuous, so it attains its extrema on $D$.

If a hypothesis fails, the theorem is unavailable; that alone does not prove nonexistence. Conversely, existence does not identify the optimizer or establish uniqueness. A later optimisation step must locate and compare valid candidates. A maximum on a boundary need not satisfy a zero ambient gradient.


## Exact result locators

- [Extreme value theorem](page-lecture-08-16.md) — Lecture 8, PDF p. 16.
- [Why its hypotheses matter](page-lecture-08-17.md) — Lecture 8, PDF p. 17.
- [Compactness](page-lecture-01-30.md) — Lecture 1, PDF p. 30.

## Further source pages

- Lecture 1, PDF pp. [30](page-lecture-01-30.md)
- Lecture 8, PDF pp. [16](page-lecture-08-16.md), [17](page-lecture-08-17.md)
- Lecture 8, PDF pp. [21](page-lecture-08-21.md), [22](page-lecture-08-22.md), [23](page-lecture-08-23.md), [24](page-lecture-08-24.md), [25](page-lecture-08-25.md)

## Official worked problems

- [Tutorial 8, Problem 3: Existence on a disk and a triangle](problem-tutorial-08-03.md)
- [Tutorial 10, Problem 2: Equality-circle constraint and existence](problem-tutorial-10-02.md)
