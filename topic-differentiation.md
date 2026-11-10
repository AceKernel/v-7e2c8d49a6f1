# Differentiability and approximation

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: partial derivatives, gradient, total differential, Taylor, marginal products.


## Partial and total derivatives

$$
f_{x_i}(a)=\lim_{t\to0}\frac{f(a+te_i)-f(a)}{t}.
$$

Hold other coordinates constant when differentiating with respect to $x_i$. Calculate the derivative before evaluating it at a requested point.

For $f:S\subseteq\mathbb R^n\to\mathbb R$, with $S$ open, total differentiability at $a$ means there is a linear map $Df(a)$ such that

$$
f(a+h)=f(a)+Df(a)h+o(\|h\|).
$$

The course identifies this map with the gradient row vector:

$$
\nabla f(a)=(f_{x_1}(a),\ldots,f_{x_n}(a)),\qquad
Df(a)h=\nabla f(a)\cdot h.
$$

Existence of all partial derivatives alone does not imply total differentiability. Continuous partial derivatives on an open neighbourhood are sufficient. Total differentiability implies continuity.

## Tangent approximation and differentials

$$
T_a(x)=f(a)+\nabla f(a)\cdot(x-a),\qquad
df=\sum_i f_{x_i}(a)\,dx_i.
$$

For a small change $h$, the approximate change is $df=\nabla f(a)\cdot h$, while the actual change is $\Delta f=f(a+h)-f(a)$. Do not identify them exactly unless $f$ is affine. For a production function, the relevant partial derivative is the marginal product, holding other inputs fixed. State its output-per-input units.


## Exact result locators

- [Total differentiability definition](page-lecture-03-10.md) — Lecture 3, PDF p. 10.
- [Partial derivative definition](page-lecture-03-14.md) — Lecture 3, PDF p. 14.
- [Gradient and total derivative](page-lecture-03-22.md) — Lecture 3, PDF p. 22.
- [First-order Taylor approximation](page-lecture-03-24.md) — Lecture 3, PDF p. 24.
- [Continuous partials imply differentiability](page-lecture-03-31.md) — Lecture 3, PDF p. 31.

## Further source pages

- Lecture 2, PDF pp. [21](page-lecture-02-21.md), [22](page-lecture-02-22.md), [23](page-lecture-02-23.md), [24](page-lecture-02-24.md), [25](page-lecture-02-25.md), [26](page-lecture-02-26.md), [27](page-lecture-02-27.md), [28](page-lecture-02-28.md), [29](page-lecture-02-29.md), [30](page-lecture-02-30.md), [31](page-lecture-02-31.md), [32](page-lecture-02-32.md), [33](page-lecture-02-33.md)
- Lecture 3, PDF pp. [2](page-lecture-03-02.md), [3](page-lecture-03-03.md), [4](page-lecture-03-04.md), [5](page-lecture-03-05.md), [6](page-lecture-03-06.md)
- Lecture 3, PDF pp. [9](page-lecture-03-09.md), [10](page-lecture-03-10.md), [11](page-lecture-03-11.md), [12](page-lecture-03-12.md), [13](page-lecture-03-13.md), [14](page-lecture-03-14.md), [15](page-lecture-03-15.md), [16](page-lecture-03-16.md), [17](page-lecture-03-17.md), [18](page-lecture-03-18.md), [19](page-lecture-03-19.md), [20](page-lecture-03-20.md), [21](page-lecture-03-21.md), [22](page-lecture-03-22.md), [23](page-lecture-03-23.md), [24](page-lecture-03-24.md), [25](page-lecture-03-25.md), [26](page-lecture-03-26.md), [27](page-lecture-03-27.md), [28](page-lecture-03-28.md), [29](page-lecture-03-29.md), [30](page-lecture-03-30.md), [31](page-lecture-03-31.md)
- Annotated revision lecture, PDF pp. [17](page-revision-lecture-17.md)

## Official worked problems

- [Tutorial 2, Problem 5: Linear and affine functions](problem-tutorial-02-05.md)
- [Tutorial 3, Problem 1: Partial derivatives and evaluation](problem-tutorial-03-01.md)
- [Tutorial 3, Problem 2: Domain, gradient, level curves and continuous differentiability](problem-tutorial-03-02.md)
- [Tutorial 3, Problem 3: A partial derivative from the definition](problem-tutorial-03-03.md)
- [Tutorial 3, Problem 4: Production differential versus actual change](problem-tutorial-03-04.md)
- [Tutorial 3, Problem 5: Chain rule for logarithmic and square-root functions](problem-tutorial-03-05.md)
- [Tutorial 4, Problem 1: First-order Taylor approximation of a logarithm](problem-tutorial-04-01.md)
