# Duality and resource values

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: weak/strong duality, complementary slackness, shadow prices, free multipliers.


## Primal and dual: row-multiplier convention

$$
\begin{array}{ll}
\text{Primal:}&\max\ c\cdot x\quad\text{s.t. }Ax\le b,\ x\ge0,\\
\text{Dual:}&\min\ y\cdot b\quad\text{s.t. }yA\ge c,\ y\ge0.
\end{array}
$$

If $A$ is $m\times n$, the dual has $m$ resource multipliers and $n$ constraints. Transpose the coefficient correspondence carefully: the dual constraint for primal variable $x_j$ uses column $j$ of $A$.

In this maximisation convention, a primal equality gives a free dual multiplier; a free primal variable gives an equality dual constraint. First standardise any reversed inequalities or minimisation objectives, rather than mixing sign conventions.

## Optimality and complementary slackness

For feasible $x,y$, weak duality gives $c\cdot x\le y\cdot b$. Feasible points with equal objective values are both optimal. Strong duality equates finite attained primal and dual optima.

$$
y_i\bigl(b_i-(Ax)_i\bigr)=0,\qquad
x_j\bigl((yA)_j-c_j\bigr)=0.
$$

For feasible primal/dual points, these conditions characterise optimality of the pair. A slack primal resource constraint has zero optimal multiplier. A binding constraint can still have a zero multiplier. If $x_j>0$, its dual constraint must bind; if $y_i>0$, its primal resource constraint must bind.

## Shadow prices and scaling

An optimal resource multiplier is the local marginal change in optimal objective value per unit of that right-hand-side resource, where the relevant value function is differentiable and the local regime persists. Hold other resources fixed and state units. A dollars-per-kilogram multiplier is not dollars per gram; rescaling a constraint rescales its multiplier inversely. Do not extrapolate a local shadow price to a large resource change without checking the active regime.


## Exact result locators

- [General dual and weak duality](page-lecture-09-12.md) — Lecture 9, PDF p. 12.
- [Strong duality](page-lecture-09-13.md) — Lecture 9, PDF p. 13.
- [Complementary slackness](page-lecture-10-02.md) — Lecture 10, PDF p. 2.
- [Shadow prices](page-lecture-09-23.md) — Lecture 9, PDF p. 23.
- [Primal equalities](page-lecture-09-24.md) — Lecture 9, PDF p. 24.
- [Free primal variables](page-lecture-09-26.md) — Lecture 9, PDF p. 26.

## Further source pages

- Lecture 9, PDF pp. [10](page-lecture-09-10.md), [11](page-lecture-09-11.md), [12](page-lecture-09-12.md), [13](page-lecture-09-13.md), [14](page-lecture-09-14.md), [15](page-lecture-09-15.md), [16](page-lecture-09-16.md), [17](page-lecture-09-17.md), [18](page-lecture-09-18.md), [19](page-lecture-09-19.md), [20](page-lecture-09-20.md), [21](page-lecture-09-21.md), [22](page-lecture-09-22.md), [23](page-lecture-09-23.md), [24](page-lecture-09-24.md), [25](page-lecture-09-25.md), [26](page-lecture-09-26.md)
- Lecture 10, PDF pp. [2](page-lecture-10-02.md), [3](page-lecture-10-03.md), [4](page-lecture-10-04.md)
- Lecture 11, PDF pp. [23](page-lecture-11-23.md), [24](page-lecture-11-24.md), [25](page-lecture-11-25.md)

## Official worked problems

- [Tutorial 9, Problem 2: Juice-factory linear program, dual and resource values](problem-tutorial-09-02.md)
- [Tutorial 9, Problem 3: A linear program and sensitivity](problem-tutorial-09-03.md)
- [Tutorial 9, Problem 4: Duals with free variables and equalities](problem-tutorial-09-04.md)
- [Tutorial 9, Problem 5: Factory operating-cost minimisation and its dual](problem-tutorial-09-05.md)
