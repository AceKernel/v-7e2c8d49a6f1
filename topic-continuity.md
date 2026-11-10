# Domains and continuity

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: log, square root, denominator, projections, compositions, sequential continuity.


## Domain first

Intersect every restriction:

$$
\ln u:\ u>0;\qquad \sqrt{u}:\ u\ge0;\qquad
\frac{v}{u}:\ u\ne0.
$$

A square root does not require a strictly positive argument merely to be defined. For a composition, the image of the inner function must lie in the domain of the outer function.

## Sequential continuity

$f:S\to\mathbb R^m$ is continuous at $a\in S$ if every sequence $(x_n)$ in $S$ with $x_n\to a$ satisfies $f(x_n)\to f(a)$.

The projections $\operatorname{pr}_i$ are continuous. Sums, differences, products and valid compositions of continuous functions are continuous; a quotient is continuous where its denominator is nonzero. Vector-valued continuity can be checked coordinatewise. Specify each component's domain before applying a closure theorem.

For example, if $u(x)\ge0$ is continuous, then $x\mapsto\sin(\sqrt{u(x)})$ is continuous by composition, since $\sqrt{\cdot}$ is continuous on $[0,\infty)$ and $\sin$ is continuous on $\mathbb R$.

## Discontinuity and extensions

One domain sequence $x_n\to a$ with $f(x_n)\not\to f(a)$ disproves continuity. To show no continuous extension exists, use two domain sequences approaching the same missing point with different function limits. Any continuous extension would have to assign both limits to that point, which is impossible.

Agreement along a few paths does not establish a multivariable limit. A proof requires a bound valid for all nearby domain points, a valid continuity theorem, or the complete definition.


## Exact result locators

- [Domain examples](page-lecture-02-03.md) — Lecture 2, PDF p. 3.
- [Sequential continuity definition](page-lecture-02-11.md) — Lecture 2, PDF p. 11.
- [Continuity algebra](page-lecture-02-16.md) — Lecture 2, PDF p. 16.
- [Continuity of composition](page-lecture-02-18.md) — Lecture 2, PDF p. 18.

## Further source pages

- Lecture 1, PDF pp. [6](page-lecture-01-06.md), [7](page-lecture-01-07.md)
- Lecture 2, PDF pp. [2](page-lecture-02-02.md), [3](page-lecture-02-03.md), [4](page-lecture-02-04.md), [5](page-lecture-02-05.md), [6](page-lecture-02-06.md), [7](page-lecture-02-07.md), [8](page-lecture-02-08.md), [9](page-lecture-02-09.md), [10](page-lecture-02-10.md), [11](page-lecture-02-11.md), [12](page-lecture-02-12.md), [13](page-lecture-02-13.md), [14](page-lecture-02-14.md), [15](page-lecture-02-15.md), [16](page-lecture-02-16.md), [17](page-lecture-02-17.md), [18](page-lecture-02-18.md), [19](page-lecture-02-19.md), [20](page-lecture-02-20.md)
- Annotated revision lecture, PDF pp. [15](page-revision-lecture-15.md), [16](page-revision-lecture-16.md)

## Official worked problems

- [Tutorial 2, Problem 1: Function statements and counterexamples](problem-tutorial-02-01.md)
- [Tutorial 2, Problem 2: Domains and level curves](problem-tutorial-02-02.md)
- [Tutorial 2, Problem 3: Continuity through projections and composition](problem-tutorial-02-03.md)
- [Tutorial 2, Problem 6: Failure of continuous extension](problem-tutorial-02-06.md)
- [Tutorial 2, Problem 7: Continuous extension across a diagonal](problem-tutorial-02-07.md)
- [Tutorial 3, Problem 2: Domain, gradient, level curves and continuous differentiability](problem-tutorial-03-02.md)
- [Tutorial 8, Problem 2: Logarithmic domain and absence of extrema](problem-tutorial-08-02.md)
