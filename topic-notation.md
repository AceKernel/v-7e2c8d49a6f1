# Notation and proof methods

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: quantifiers, contradiction, contrapositive, positive orthants, vector inequalities.


## Course notation

$$
\mathbb N=\{1,2,3,\ldots\},\qquad
\mathbb R_+=[0,\infty),\qquad \mathbb R_{++}=(0,\infty).
$$

For vectors, $y\ge z$ means $y_i\ge z_i$ for every $i$; $y>z$ means $y\ge z$ and $y\ne z$; $y\gg z$ means $y_i>z_i$ for every $i$. In particular, $x>0$ does not require every coordinate to be positive. Use $\mathbb R_{++}^n$ or $x\gg0$ when that is intended.

$$
A\times B=\{(a,b):a\in A,\ b\in B\},\quad
A\setminus B=\{x\in A:x\notin B\},\quad
\|x\|=\sqrt{\sum_{i=1}^n x_i^2}.
$$

Use $|t|$ for a scalar and $\|x\|$ for a vector. Distinguish a function's domain, codomain and image; state $f:S\to\mathbb R$, not only its formula. The projections are $\operatorname{pr}_i(x)=x_i$.

## Definition-proof pattern

Choose arbitrary quantified objects, state the relevant definition, establish the required inequality or implication, then conclude for all objects chosen. To disprove a universal claim, give one valid counterexample.

$$
\neg(\forall x\in S\ P(x))\iff\exists x\in S\ \neg P(x),\qquad
\neg(\exists x\in S\ P(x))\iff\forall x\in S\ \neg P(x).
$$

The contrapositive of $P\Rightarrow Q$ is $\neg Q\Rightarrow\neg P$, not its converse. In a contradiction proof, identify the assumption being contradicted. Keep strict and weak inequalities distinct.


## Exact result locators

- [Positive orthants and set difference](page-notation-03.md) — Notation, PDF p. 3.
- [Negating quantifiers](page-logic-03.md) — Logic, PDF p. 3.
- [Vector inequality convention](page-lecture-06-03.md) — Lecture 6, PDF p. 3.

## Further source pages

- Logic, PDF pp. [1](page-logic-01.md), [2](page-logic-02.md), [3](page-logic-03.md), [4](page-logic-04.md), [5](page-logic-05.md)
- Notation, PDF pp. [1](page-notation-01.md), [2](page-notation-02.md), [3](page-notation-03.md), [4](page-notation-04.md)
- Lecture 6, PDF pp. [3](page-lecture-06-03.md)

## Official worked problems

- [Tutorial 2, Problem 1: Function statements and counterexamples](problem-tutorial-02-01.md)
