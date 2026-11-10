# Nonnegative-variable KKT

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: reduced Lagrangian, complementary slackness, corners, global sufficiency.


## Reduced KKT for nonnegative variables

For the course problem

$$
\max f(x)\quad\text{s.t. }g_j(x)\le0,\quad x\ge0,
$$

define $L(x,\lambda)=f(x)-\sum_j\lambda_jg_j(x)$, omitting explicit multipliers for $x_i\ge0$. The reduced conditions retain their effect:

$$
\begin{aligned}
L_{x_i}(x,\lambda)&\le0,&x_iL_{x_i}(x,\lambda)&=0,&x_i&\ge0,\\
g_j(x)&\le0,&\lambda_jg_j(x)&=0,&\lambda_j&\ge0.
\end{aligned}
$$

If $x_i>0$, then $L_{x_i}=0$; if $x_i=0$, only $L_{x_i}\le0$ is required. Setting every reduced derivative equal to zero can lose corner candidates. Equivalently, the full Lagrangian includes $+\nu_i x_i$ with $\nu_i\ge0$ and stationarity $L_{x_i}+\nu_i=0$.

## Procedure and justification

Check domain and existence where appropriate. For necessity, verify continuous differentiability on an open ambient domain and either affine constraints or the relevant active-gradient qualification, including the gradients of active nonnegativity constraints. Enumerate positive/zero variables and binding/slack resource constraints. Solve each case, then check feasibility, derivative inequalities, multiplier signs and complementary slackness. Retain qualification-failure candidates when needed.

For global sufficiency, use a convex ambient domain, a continuously differentiable concave objective and continuously differentiable convex inequality functions. A feasible KKT point then maximises globally; strict concavity on the convex feasible set gives uniqueness. Equality constraints, if included, require their own free multipliers and affine form for this sufficiency result.

The complementary product is $x_iL_{x_i}=0$ as derived from the full conditions; do not reproduce the isolated typesetting error in Lecture 11 PDF page 18.


## Exact result locators

- [Reduced KKT conditions](page-lecture-11-05.md) — Lecture 11, PDF p. 5.
- [Necessity and active nonnegativity](page-lecture-11-07.md) — Lecture 11, PDF p. 7.
- [Candidate procedure](page-lecture-11-09.md) — Lecture 11, PDF p. 9.
- [Sufficiency: use the correctly derived complementary product](page-lecture-11-18.md) — Lecture 11, PDF p. 18.

## Further source pages

- Lecture 11, PDF pp. [2](page-lecture-11-02.md), [3](page-lecture-11-03.md), [4](page-lecture-11-04.md), [5](page-lecture-11-05.md), [6](page-lecture-11-06.md), [7](page-lecture-11-07.md), [8](page-lecture-11-08.md), [9](page-lecture-11-09.md), [10](page-lecture-11-10.md), [11](page-lecture-11-11.md), [12](page-lecture-11-12.md), [13](page-lecture-11-13.md), [14](page-lecture-11-14.md), [15](page-lecture-11-15.md), [16](page-lecture-11-16.md), [17](page-lecture-11-17.md), [18](page-lecture-11-18.md), [19](page-lecture-11-19.md), [20](page-lecture-11-20.md), [21](page-lecture-11-21.md), [22](page-lecture-11-22.md), [23](page-lecture-11-23.md), [24](page-lecture-11-24.md), [25](page-lecture-11-25.md)

## Official worked problems

- [Tutorial 11, Problem 1: Nonnegative KKT with linear constraints](problem-tutorial-11-01.md)
- [Tutorial 11, Problem 2: Cobb-Douglas choice and an increasing transformation](problem-tutorial-11-02.md)
- [Tutorial 11, Problem 3: Quadratic concavity and KKT sufficiency](problem-tutorial-11-03.md)
