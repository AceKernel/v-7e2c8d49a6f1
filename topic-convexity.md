# Convexity and concavity

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: convex sets, strict convexity, weighted sums, composition, epigraph, hypograph.


## Definitions

$S$ is convex if $\lambda x+(1-\lambda)y\in S$ whenever $x,y\in S$ and $\lambda\in[0,1]$. On a convex domain $S$, $f$ is convex if

$$
f(\lambda x+(1-\lambda)y)
\le\lambda f(x)+(1-\lambda)f(y).
$$

Concavity reverses the inequality. Strict convexity/concavity requires a strict inequality for $x\ne y$ and $0<\lambda<1$. An affine function is both convex and concave.

For a definition proof, choose arbitrary $x,y,\lambda$, verify the convex combination is in the domain, and derive the defining inequality. For a finite sum of convex functions, sum their inequalities and factor out $\lambda$ and $1-\lambda$; do not replace a requested definition proof with a derivative test.

## Course closure results

Nonnegative weighted sums preserve convexity/concavity; negation exchanges them. An increasing convex outer function composed with a convex inner function is convex; an increasing concave outer function composed with a concave inner function is concave. An affine inner function permits either convex or concave outer functions without a monotonicity assumption, on a valid convex domain.

For a twice differentiable function on an open interval, $f''\ge0$ characterises convexity and $f''\le0$ concavity; strict signs suffice for strict curvature but are not necessary everywhere.

For continuously differentiable $f$ on an open convex domain, concavity is equivalent to

$$
f(x)-f(a)\le\nabla f(a)\cdot(x-a)\quad(a,x\in S);
$$

reverse this for convexity. Concave graphs lie below their tangent hyperplanes; convex graphs lie above.

$$
\operatorname{epi}f=\{(x,t):x\in S,\ t\ge f(x)\},\quad
\operatorname{hyp}f=\{(x,t):x\in S,\ t\le f(x)\}.
$$

Convexity of $f$ is equivalent to convexity of its epigraph; concavity to convexity of its hypograph. Convex-function sublevel sets and concave-function superlevel sets are convex. Intersections of convex sets are convex; unions need not be.


## Exact result locators

- [Convex-set definition](page-lecture-07-04.md) — Lecture 7, PDF p. 4.
- [Convex-function definition](page-lecture-07-09.md) — Lecture 7, PDF p. 9.
- [Concavity and strictness](page-lecture-07-11.md) — Lecture 7, PDF p. 11.
- [Weighted sums and negation](page-lecture-07-17.md) — Lecture 7, PDF p. 17.
- [Composition](page-lecture-07-18.md) — Lecture 7, PDF p. 18.
- [First-order characterisation](page-lecture-07-26.md) — Lecture 7, PDF p. 26.

## Further source pages

- Lecture 7, PDF pp. [2](page-lecture-07-02.md), [3](page-lecture-07-03.md), [4](page-lecture-07-04.md), [5](page-lecture-07-05.md), [6](page-lecture-07-06.md), [7](page-lecture-07-07.md), [8](page-lecture-07-08.md), [9](page-lecture-07-09.md), [10](page-lecture-07-10.md), [11](page-lecture-07-11.md), [12](page-lecture-07-12.md), [13](page-lecture-07-13.md), [14](page-lecture-07-14.md), [15](page-lecture-07-15.md), [16](page-lecture-07-16.md), [17](page-lecture-07-17.md), [18](page-lecture-07-18.md), [19](page-lecture-07-19.md), [20](page-lecture-07-20.md), [21](page-lecture-07-21.md), [22](page-lecture-07-22.md), [23](page-lecture-07-23.md), [24](page-lecture-07-24.md), [25](page-lecture-07-25.md), [26](page-lecture-07-26.md), [27](page-lecture-07-27.md), [28](page-lecture-07-28.md), [29](page-lecture-07-29.md), [30](page-lecture-07-30.md)
- Lecture 8, PDF pp. [12](page-lecture-08-12.md), [13](page-lecture-08-13.md), [14](page-lecture-08-14.md), [15](page-lecture-08-15.md)
- Lecture 11, PDF pp. [15](page-lecture-11-15.md), [16](page-lecture-11-16.md), [17](page-lecture-11-17.md), [18](page-lecture-11-18.md), [19](page-lecture-11-19.md), [20](page-lecture-11-20.md), [21](page-lecture-11-21.md), [22](page-lecture-11-22.md)
- Annotated revision lecture, PDF pp. [13](page-revision-lecture-13.md), [14](page-revision-lecture-14.md)

## Official worked problems

- [Tutorial 7, Problem 1: Convexity of sublevel sets from the definition](problem-tutorial-07-01.md)
- [Tutorial 7, Problem 2: Convexity of a separable sum](problem-tutorial-07-02.md)
- [Tutorial 7, Problem 3: Convexity of intersecting constraint sets](problem-tutorial-07-03.md)
- [Tutorial 7, Problem 4: Convexity and concavity by composition](problem-tutorial-07-04.md)
- [Tutorial 7, Problem 5: Strict convexity of a square from the definition](problem-tutorial-07-05.md)
- [Tutorial 7, Problem 6: Intersections of convex sets: extra practice](problem-tutorial-07-06.md)
- [Tutorial 8, Problem 1: Affine-inner composition, quadratic curvature and extrema](problem-tutorial-08-01.md)
- [Tutorial 8, Problem 4: Quadratic profit and a global maximum](problem-tutorial-08-04.md)
- [Tutorial 11, Problem 3: Quadratic concavity and KKT sufficiency](problem-tutorial-11-03.md)
