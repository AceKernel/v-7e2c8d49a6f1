# Graphs and diagrams

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: TikZ, level curves, included/excluded boundary, feasible set, cone.


## Course-style mathematical sketches

Use the question's variable names and axis orientation; arrowed labelled axes; exact intercepts and relevant intersections; light shading labelled with the set name. Included boundaries are solid and excluded boundaries dashed. Filled/open markers must reflect membership in the entire set, including other constraints. Preserve holes, separate components and unbounded directions.

Use equal axis units where geometry, circles or distance matter. An enclosing rectangle is a bound, not necessarily the feasible set. A pairwise line intersection is not an LP vertex until it satisfies every constraint. State exact boundary equations and key coordinates beside a hand-reproducible sketch.

See [original graph examples and presentation details](GRAPH-STYLE.md). Tutorial 8 illustrates domains and compact sets; Tutorial 9 illustrates feasible polygons. Colour is optional; solid/dashed boundaries and shading must remain clear in monochrome.

## TikZ template

For requested diagrams, use a complete `tikzpicture` outside ordinary equation delimiters. This basic-primitives example depicts Tutorial 8's closed triangle $x+2y\le3$, $x,y\ge0$; adapt equations and vertices rather than copying the shape for a different problem.

```latex
\begin{tikzpicture}[x=1cm,y=1cm]
  \fill[gray!15] (0,0)--(3,0)--(0,1.5)--cycle;
  \draw[->] (-0.3,0)--(3.7,0) node[right] {$x$};
  \draw[->] (0,-0.3)--(0,2.2) node[above] {$y$};
  \draw[thick] (0,0)--(3,0)--(0,1.5)--cycle;
  \node[below left] at (0,0) {$O$};
  \node[below] at (3,0) {$(3,0)$};
  \node[left] at (0,1.5) {$(0,\frac32)$};
  \node[above right] at (1.5,0.75) {$x+2y=3$};
  \node at (0.8,0.45) {$D$};
\end{tikzpicture}
```

This requires the standard TikZ package in a LaTeX document. Code is not a claim that a particular external renderer supports it. If rendering is unavailable, retain exact sketch instructions and coordinates.


## Exact result locators

- [Excluded parabola and included disk](page-tutorial-08-solutions-03.md) — Tutorial 8 solutions, PDF p. 3.
- [Closed triangle](page-tutorial-08-solutions-04.md) — Tutorial 8 solutions, PDF p. 4.
- [Feasible polygon and labelled vertices](page-tutorial-09-solutions-03.md) — Tutorial 9 solutions, PDF p. 3.

## Further source pages

- Lecture 1, PDF pp. [19](page-lecture-01-19.md), [20](page-lecture-01-20.md)
- Lecture 2, PDF pp. [4](page-lecture-02-04.md), [5](page-lecture-02-05.md), [6](page-lecture-02-06.md), [7](page-lecture-02-07.md), [8](page-lecture-02-08.md), [9](page-lecture-02-09.md)
- Lecture 4, PDF pp. [15](page-lecture-04-15.md), [16](page-lecture-04-16.md), [17](page-lecture-04-17.md), [18](page-lecture-04-18.md), [19](page-lecture-04-19.md), [20](page-lecture-04-20.md), [21](page-lecture-04-21.md), [22](page-lecture-04-22.md)
- Lecture 6, PDF pp. [5](page-lecture-06-05.md), [6](page-lecture-06-06.md), [7](page-lecture-06-07.md), [8](page-lecture-06-08.md), [9](page-lecture-06-09.md), [10](page-lecture-06-10.md), [11](page-lecture-06-11.md), [12](page-lecture-06-12.md), [13](page-lecture-06-13.md), [14](page-lecture-06-14.md)
- Lecture 9, PDF pp. [3](page-lecture-09-03.md), [4](page-lecture-09-04.md), [5](page-lecture-09-05.md)
- Annotated revision lecture, PDF pp. [15](page-revision-lecture-15.md), [16](page-revision-lecture-16.md)

## Official worked problems

- [Tutorial 2, Problem 2: Domains and level curves](problem-tutorial-02-02.md)
- [Tutorial 2, Problem 4: Production isoquants](problem-tutorial-02-04.md)
- [Tutorial 3, Problem 2: Domain, gradient, level curves and continuous differentiability](problem-tutorial-03-02.md)
- [Tutorial 4, Problem 4: Tangent lines to implicit level curves](problem-tutorial-04-04.md)
- [Tutorial 6, Problem 1: Cones, sub-cones and nonnegative feasibility](problem-tutorial-06-01.md)
- [Tutorial 8, Problem 3: Existence on a disk and a triangle](problem-tutorial-08-03.md)
- [Tutorial 9, Problem 1: Graphical optimisation on different feasible sets](problem-tutorial-09-01.md)
- [Tutorial 9, Problem 2: Juice-factory linear program, dual and resource values](problem-tutorial-09-02.md)
