# Chain rule and Hessians

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: composite derivatives, second partials, Young theorem.


## Chain rules

For a differentiable path $x(t)=(x_1(t),\ldots,x_n(t))$ and differentiable $f$,

$$
\frac{d}{dt}f(x(t))=
\sum_{i=1}^n f_{x_i}(x(t))x_i'(t).
$$

For inner coordinates depending on $s,t$,

$$
\frac{\partial}{\partial s}f(x_1(s,t),\ldots,x_n(s,t))
=\sum_{i=1}^n f_{x_i}(x(s,t))\frac{\partial x_i}{\partial s}(s,t).
$$

State which quantities depend on the differentiation variable. Include every changing inner coordinate; do not treat an indirect dependence as constant. Substitute evaluation points only after forming the derivative.

## Second partials and Hessian

Using row $i$, column $j$ for $\partial_{x_j}(\partial_{x_i}f)$,

$$
Hf=\begin{pmatrix}
f_{xx}&f_{xy}\\
f_{yx}&f_{yy}
\end{pmatrix}
\quad\text{in two variables}.
$$

Young's theorem: if the second partial derivatives are continuous on an open neighbourhood, the mixed partials agree there. Verify the regularity hypothesis; merely obtaining equal expressions in one calculation is not the theorem's hypothesis.

Differentiate products and quotients carefully, keep a consistent variable order, and state the valid domain. Symmetry of a Hessian does not by itself establish convexity, concavity or an extremum. Use the curvature method requested in the question; the course gives definition and composition methods in [convexity](topic-convexity.md).


## Exact result locators

- [Chain rule along a curve](page-lecture-04-04.md) — Lecture 4, PDF p. 4.
- [Multivariable chain rule](page-lecture-04-07.md) — Lecture 4, PDF p. 7.
- [Young theorem](page-lecture-04-12.md) — Lecture 4, PDF p. 12.
- [Hessian matrix](page-lecture-04-13.md) — Lecture 4, PDF p. 13.

## Further source pages

- Lecture 3, PDF pp. [7](page-lecture-03-07.md), [8](page-lecture-03-08.md)
- Lecture 4, PDF pp. [2](page-lecture-04-02.md), [3](page-lecture-04-03.md), [4](page-lecture-04-04.md), [5](page-lecture-04-05.md), [6](page-lecture-04-06.md), [7](page-lecture-04-07.md), [8](page-lecture-04-08.md), [9](page-lecture-04-09.md), [10](page-lecture-04-10.md), [11](page-lecture-04-11.md), [12](page-lecture-04-12.md), [13](page-lecture-04-13.md), [14](page-lecture-04-14.md)
- Annotated revision lecture, PDF pp. [17](page-revision-lecture-17.md)

## Official worked problems

- [Tutorial 3, Problem 5: Chain rule for logarithmic and square-root functions](problem-tutorial-03-05.md)
- [Tutorial 4, Problem 2: Chain rule along a parametrised curve](problem-tutorial-04-02.md)
- [Tutorial 4, Problem 5: Hessian calculations](problem-tutorial-04-05.md)
