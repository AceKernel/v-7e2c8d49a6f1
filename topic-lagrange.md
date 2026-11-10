# Lagrange multipliers

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: stationarity, active constraints, LICQ, equality constraints, necessity and sufficiency.


## Maximisation sign convention

For $\max f(x)$ with $g_j(x)\le0$ and $h_k(x)=0$, the course convention is

$$
L(x,\lambda,\mu)=f(x)-\sum_j\lambda_jg_j(x)-\sum_k\mu_kh_k(x),
\qquad \lambda_j\ge0,\quad \mu_k\in\mathbb R.
$$

The conditions are

$$
\nabla_xL=0,\quad g_j\le0,\quad h_k=0,\quad
\lambda_j\ge0,\quad \lambda_jg_j=0.
$$

Equality multipliers are unrestricted. For minimisation, maximise $-f$ before using these signs. A constraint written $a(x)\ge b$ becomes $g(x)=b-a(x)\le0$.

## Necessity and complete cases

Use the course necessity theorem on an open domain with continuously differentiable objective and constraints. It applies when the constraints are affine, or when the gradients of active constraints satisfy the stated linear-independence qualification. Equality constraints are active. Include active nonnegativity constraints if present.

Enumerate binding/slack cases using complementary slackness. Solve stationarity and binding equalities; check all domain restrictions, primal feasibility and multiplier signs. Do not rule out an optimum merely because multipliers fail at a qualification-failure point: retain such points for the complete candidate comparison when required.

For a compact feasible set, establish existence and compare the full candidate set. Necessary equations alone do not establish global optimality.

## Global sufficiency

On a convex ambient domain, with continuously differentiable concave $f$, convex inequality functions $g_j$, and affine equalities $h_k$, a feasible point and multipliers satisfying these conditions give a global maximum. Strict concavity gives uniqueness on the convex feasible set. Distinguish this sufficiency theorem from the constraint-qualification theorem used for necessity.


## Exact result locators

- [Necessity with affine constraints](page-lecture-10-13.md) — Lecture 10, PDF p. 13.
- [Active-gradient qualification](page-lecture-10-15.md) — Lecture 10, PDF p. 15.
- [Equality theorem](page-lecture-10-25.md) — Lecture 10, PDF p. 25.
- [Mixed constraints](page-lecture-10-28.md) — Lecture 10, PDF p. 28.
- [Global sufficiency](page-lecture-11-16.md) — Lecture 11, PDF p. 16.
- [Affine equality sufficiency](page-lecture-11-20.md) — Lecture 11, PDF p. 20.

## Further source pages

- Lecture 10, PDF pp. [5](page-lecture-10-05.md), [6](page-lecture-10-06.md), [7](page-lecture-10-07.md), [8](page-lecture-10-08.md), [9](page-lecture-10-09.md), [10](page-lecture-10-10.md), [11](page-lecture-10-11.md), [12](page-lecture-10-12.md), [13](page-lecture-10-13.md), [14](page-lecture-10-14.md), [15](page-lecture-10-15.md), [16](page-lecture-10-16.md), [17](page-lecture-10-17.md), [18](page-lecture-10-18.md), [19](page-lecture-10-19.md), [20](page-lecture-10-20.md), [21](page-lecture-10-21.md), [22](page-lecture-10-22.md), [23](page-lecture-10-23.md), [24](page-lecture-10-24.md), [25](page-lecture-10-25.md), [26](page-lecture-10-26.md), [27](page-lecture-10-27.md), [28](page-lecture-10-28.md)
- Lecture 11, PDF pp. [15](page-lecture-11-15.md), [16](page-lecture-11-16.md), [17](page-lecture-11-17.md), [18](page-lecture-11-18.md), [19](page-lecture-11-19.md), [20](page-lecture-11-20.md), [21](page-lecture-11-21.md), [22](page-lecture-11-22.md)

## Official worked problems

- [Tutorial 10, Problem 1: Affine-constraint Lagrange cases](problem-tutorial-10-01.md)
- [Tutorial 10, Problem 2: Equality-circle constraint and existence](problem-tutorial-10-02.md)
- [Tutorial 10, Problem 3: Log utility with a quadratic equality and multiplier interpretation](problem-tutorial-10-03.md)
- [Tutorial 10, Problem 4: Parameter-dependent disk constraint: extra practice](problem-tutorial-10-04.md)
- [Tutorial 11, Problem 3: Quadratic concavity and KKT sufficiency](problem-tutorial-11-03.md)
