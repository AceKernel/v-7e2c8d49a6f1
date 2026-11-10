# Sets and compactness

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: open balls, interior, exterior, boundary, closed, bounded.


## Definitions in $\mathbb R^n$

$$
B_r(a)=\{x\in\mathbb R^n:\|x-a\|<r\},\qquad r>0.
$$

- $a$ is interior to $D$ if some $B_r(a)\subseteq D$.
- $a$ is exterior to $D$ if some $B_r(a)\cap D=\varnothing$.
- $a$ is a boundary point if every $B_r(a)$ meets both $D$ and $\mathbb R^n\setminus D$.

$D$ is open when every point in $D$ is interior; it is closed when it contains all its boundary points. A boundary point need not belong to $D$.

$$
D\text{ bounded}\iff\exists M>0\ \forall x\in D:\|x\|\le M.
$$

In Euclidean space, compact means closed and bounded. Nonemptiness is an additional requirement when applying the extreme value theorem.

## Classification and drawing

Identify the actual feasible region, then determine its interior and boundary. An intersection of closed half-spaces is closed. A strict inequality may exclude a boundary piece, but do not classify a set solely by the symbols appearing in its description: constraints can be redundant, or the set empty.

To prove a point outside $D$ is exterior, exhibit a positive radius whose ball misses $D$. To disprove openness, give a point in $D$ with no contained ball. To disprove closedness, give an excluded boundary point or a sequence in $D$ converging outside it.

In a sketch, use solid included boundaries, dashed excluded boundaries and correct endpoint markers. State interior and boundary sets algebraically, not only pictorially. See [graph conventions](topic-graphs.md).


## Exact result locators

- [Interior, exterior and boundary definitions](page-lecture-01-26.md) — Lecture 1, PDF p. 26.
- [Open and closed sets](page-lecture-01-27.md) — Lecture 1, PDF p. 27.
- [Boundedness and compactness](page-lecture-01-30.md) — Lecture 1, PDF p. 30.

## Further source pages

- Lecture 1, PDF pp. [18](page-lecture-01-18.md), [19](page-lecture-01-19.md), [20](page-lecture-01-20.md)
- Lecture 1, PDF pp. [26](page-lecture-01-26.md), [27](page-lecture-01-27.md), [28](page-lecture-01-28.md), [29](page-lecture-01-29.md), [30](page-lecture-01-30.md)
- Annotated revision lecture, PDF pp. [15](page-revision-lecture-15.md), [16](page-revision-lecture-16.md)
