# Linear programming

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: standard form, feasible polygon, extreme points, binding and slack.


## Course maximisation standard form

$$
\max_{x\in\mathbb R^n}c\cdot x
\quad\text{subject to }Ax\le b,\quad x\ge0.
$$

Declare each decision variable and units. Convert all resources to consistent units before forming constraints and the profit/revenue/cost objective. Do not add integer restrictions unless the question asks for an integer program; the course LP is over real vectors. If the resulting optimum is integral, it also solves the corresponding whole-unit choice.

## Graphical solution

1. Draw and label each constraint line and the correct feasible side, including nonnegativity.
2. Solve relevant pairwise intersections and intercepts algebraically.
3. Check every candidate against **all** constraints; a line intersection may be infeasible.
4. List the feasible polygon's vertices and evaluate $c\cdot x$ at each.
5. State the optimal quantities, maximum value and units.

The fundamental theorem used in the course: if a standard-form LP has an optimal solution, at least one feasible extreme point is optimal. It does not say every optimum is a vertex; an entire edge can be optimal.

For existence on a nonempty bounded feasible polygon, justify closedness and continuity and apply the extreme value theorem. An LP may instead be infeasible or unbounded; do not assume attainment before checking.

A resource constraint is binding at $x^*$ when $(Ax^*)_i=b_i$; it is slack when $(Ax^*)_i<b_i$. Its numerical slack is $b_i-(Ax^*)_i$, in the resource's units. Nonnegativity is binding if $x_j^*=0$ and slack if $x_j^*>0$.

For duals, sensitivity and optimality certificates, use [duality](topic-duality.md).


## Exact result locators

- [Standard form and binding/slack](page-lecture-09-07.md) — Lecture 9, PDF p. 7.
- [Fundamental theorem](page-lecture-09-09.md) — Lecture 9, PDF p. 9.
- [Example feasible polygon](page-lecture-09-04.md) — Lecture 9, PDF p. 4.

## Further source pages

- Lecture 9, PDF pp. [2](page-lecture-09-02.md), [3](page-lecture-09-03.md), [4](page-lecture-09-04.md), [5](page-lecture-09-05.md), [6](page-lecture-09-06.md), [7](page-lecture-09-07.md), [8](page-lecture-09-08.md), [9](page-lecture-09-09.md)

## Official worked problems

- [Tutorial 9, Problem 2: Juice-factory linear program, dual and resource values](problem-tutorial-09-02.md)
- [Tutorial 9, Problem 3: A linear program and sensitivity](problem-tutorial-09-03.md)
