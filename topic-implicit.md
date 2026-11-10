# Implicit functions

[Index](INDEX.md) | [Course guide](COURSE-GUIDE.md)

> Reviewed supplementary reference, not official teaching material or an answer key. Mathematical expressions below are LaTeX, unlike automatic source extracts. Check the precise hypotheses and any official corrections.

Search terms: level curves, implicit differentiation, tangent lines, comparative statics.


## Local implicit representation

Consider $G(x,y)=C$ at $(x_0,y_0)$. Check:

1. $G(x_0,y_0)=C$.
2. $G$ is continuously differentiable on an open neighbourhood.
3. $G_y(x_0,y_0)\ne0$.

The implicit function theorem then gives a local continuously differentiable function $y=g(x)$ with $g(x_0)=y_0$ and $G(x,g(x))=C$.

$$
g'(x_0)=-\frac{G_x(x_0,y_0)}{G_y(x_0,y_0)},\qquad
y=y_0+g'(x_0)(x-x_0)
$$

is the tangent-line equation.

For $x=(x_1,\ldots,x_m)$ and scalar $y$, the corresponding local formula is

$$
\frac{\partial g}{\partial x_i}(x_0)
=-\frac{G_{x_i}(x_0,y_0)}{G_y(x_0,y_0)}.
$$

When differentiating $G(x,g(x))=C$, include the derivative of $g$ in every term where $y$ changes. For a three-variable level set solved as $z=g(x,y)$, use $g_x=-G_x/G_z$ and $g_y=-G_y/G_z$ at a point where $G_z\ne0$.

If the denominator is zero, this theorem does not certify that representation; it does not automatically prove that no implicit representation exists. Check whether a different dependent variable is permitted. The conclusion is local, not a global solution of the whole level set.


## Exact result locators

- [Two-variable implicit function theorem](page-lecture-04-19.md) — Lecture 4, PDF p. 19.
- [Several-input implicit theorem](page-lecture-04-24.md) — Lecture 4, PDF p. 24.
- [Worked implicit slope](page-lecture-04-22.md) — Lecture 4, PDF p. 22.

## Further source pages

- Lecture 4, PDF pp. [15](page-lecture-04-15.md), [16](page-lecture-04-16.md), [17](page-lecture-04-17.md), [18](page-lecture-04-18.md), [19](page-lecture-04-19.md), [20](page-lecture-04-20.md), [21](page-lecture-04-21.md), [22](page-lecture-04-22.md), [23](page-lecture-04-23.md), [24](page-lecture-04-24.md), [25](page-lecture-04-25.md)

## Official worked problems

- [Tutorial 4, Problem 3: Implicit partial derivatives](problem-tutorial-04-03.md)
- [Tutorial 4, Problem 4: Tangent lines to implicit level curves](problem-tutorial-04-04.md)
- [Tutorial 4, Problem 6: Implicit total derivative on a sphere](problem-tutorial-04-06.md)
