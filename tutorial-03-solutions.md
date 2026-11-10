# Tutorial 3 solutions: automatic text transcript

Original: [Tutorial 3 solutions PDF](tutorial-03-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON2050
S2 2026
Tutorial 3 Solution
Problem 1
(a) Let
f : R3
++ →R, (x1, x2, x3) 7→3x2
1 + ex2
2x3
.
Compute all partial derivatives.
(b) Evaluate the partial derivative of f with respect to x3 at the point (1, 2, 3).
Solution:
(a) The partial derivatives are
∂f(x1, x2, x3)
∂x1
= 3x1
x3
∂f(x1, x2, x3)
∂x2
= ex2
2x3
∂f(x1, x2, x3)
∂x3
= −3x2
1 −ex2
2x2
3
To derive them, simply hold all other variables constant. This allows you to treat
the function as a function of one variable—the one you are differentiating with
respect to—and apply the rules of differentiation for functions of one variables at
the beginning of Lecture 3 slides.
(b) We obtain
∂f(1, 2, 3)
∂x3
= −3 · 12 −e2
2 · 32
= −3 −e2
18
.
Problem 2
You are given the function f : D →R, (x, y) 7→e
x
y + ln(x2 + 1), where D is the
largest subset of R2 on which f is well-defined.
(a) Determine D.
Solution: The domain of f is D = {(x, y) ∈R2 : y ̸= 0}: if y = 0, e
x
y is not
well-defined.
1
```

## PDF page 2

```text
(b) Recall that the gradient ∇f(x, y) of f at (x, y) is defined as ∇f(x, y) =

∂f(x,y)
∂x
, ∂f(x,y)
∂y

.
Calculate the gradient of f at every point (x, y).
Solution: We first determine f’s partial derivatives as
∂f(x, y)
∂x
= 1
ye
x
y +
2x
x2 + 1,
∂f(x, y)
∂y
= −x
y2e
x
y .
Then, the gradient of f at (x, y) is
∇f(x, y) =
1
ye
x
y +
2x
x2 + 1, −x
y2e
x
y

(c) Show that all points of the form (0, y), y ̸= 0, are located on the same level curve.
Solution: For every point (0, y) such that y ̸= 0
f(0, y) = e
0
y + ln(0 + 1) = e0 + ln(1) = 1 + 0 = 1.
Hence, f(0, y) does not depend on y, and all points of the form (0, y) are on the
level curve of level 1.
(d) (Harder) Determine, without checking the definition directly, whether f(x, y) is
continuously differentiable at the point (1, 1).
Solution: Recall a theorem in the lecture saying that if a function is continuously
partially differentiable, then it is (totally) differentiable. It now suffices to check
that both ∂f(x,y)
∂x
and ∂f(x,y)
∂y
are continuous at the point (1, 1). To show continuity,
we use the properties of continuous function described in the slides of Lecture 2.
Observe that both ∂f(x,y)
∂x
and ∂f(x,y)
∂y
are well-defined around (1, 1), and
∂f(x, y)
∂x
= 1
pr2
· e
pr1
pr2 +
2pr1
(pr1)2 + 1;
because ex, pr1, and pr2 are continuous, and the relevant operations (sum, prod-
uct, quotient, and composition) preserve continuity, we conclude that ∂f(x,y)
∂x
is
continuous at (1, 1). Similarly,
∂f(x, y)
∂y
= −pr1
(pr2)2 · e
pr1
pr2 ,
which is also continuous by an analogous argument.
2
```

## PDF page 3

```text
Problem 3
Consider the function f : R2 →R, (x, y) 7→
xy
x2+y2+1. Determine ∂f(1,1)
∂x
directly
from the definition of the partial derivative, that is, by calculating the appropriate
limit.
Solution: We obtain
∂f(1, 1)
∂x
= lim
n→∞
f(1 + hn, 1) −f(1, 1)
hn
= lim
n→∞
1+hn
2+(1+hn)2 −1
3
hn
= lim
n→∞
3 + 3hn −2 −(1 + hn)2
3hn(2 + (1 + hn)2)
= lim
n→∞
hn(1 −hn)
3hn(2 + (1 + hn)2)
= lim
n→∞
(1 −hn)
3(2 + (1 + hn)2) = 1
9.
You are encouraged to check that if we derive the partial derivatives using the rules
of one-variable calculus by “holding other variables constant,” we get the same result.
Problem 4
The production function of a firm is f : R2
+ →R, (K, L) 7→4K
3
4L
1
4. Currently,
the firm is using 10,000 units of capital (K) and employing 625 workers (L). The CEO
of the firm would like to know how the production of output (f(L, K)) changes when
the capital is increased by one unit and one more worker is employed. Can you help
her?
Solution: In order to compute the change in the output production level, we can use
derivatives (keep in mind that this approach provides an approximation of the exact
answer). If capital changes by dK = 1 and labor by dL = 1, then the output will
change by
∆f ≈df = ∂f(10000, 625)
∂K
· dK + ∂f(10000, 625)
∂L
· dL.
From
∂f(K, L)
∂K
= 43
4K−1/4L1/4 = 3
4
4K3/4L1/4
K
= 3
4
f(K, L)
K
,
∂f(K, L)
∂L
= 41
4K3/4L−3/4 = 1
4
4K3/4L1/4
L
= 1
4
f(K, L)
L
,
3
```

## PDF page 4

```text
and
f(10000, 625) = 4(10000)3/4(625)1/4 = 4 · 1000 · 5 = 20000
we obtain
∂f(10000, 625)
∂K
= 3
4
20000
10000 = 3
2,
∂f(10000, 625)
∂L
= 1
4
20000
625
= 8,
and can conclude that the production of output increases by
∆f ≈df = 3
2 · dK + 8 · dL = 9.5
units.
Alternatively, we can compute the value of the production function for the old
and the new values of K and L and compute the difference. Currently, the firm
employs K = 10000 units of capital, L = 625 units of labor, and, as we saw above,
produces f(10000, 625) = 20000 units of output. With the increased amounts of
capital and labor, the firm would produce
f(10001, 626) = 4(10001)3/4(626)1/4 ≈20009.4958
units of output. Hence, increasing the input of both capital and labor by 1 unit each
increases output by approximately 9.4958 units.
(Just looking at this particular question, it may seem that the second approach
is actually easier, and that our efforts to understand derivatives are not paying off.
However, soon, when we discuss how to optimize [= maximize or minimize] func-
tions, this changes dramatically. For optimization problems, approaches using deriva-
tives will be “easy,” while those relying on just computing different values for f will
be cumbersome or even not viable.)
Problem 5 (Extra Practice Problem)
For each of the following functions f, calculate the partial derivatives, and eval-
uate them at the point (1, 1).
(a) f : R2 →R, (x, y) 7→ln(x2 + y2 + 1)
(b) f : R2
++ →R, (x, y) 7→
p
xy + y3
Solution:
(a) To find ∂f(x,y)
∂x
, we treat y as a constant, and use the chain rule:
1. Take the derivative of the outer function, ln(u), where u ≡x2 +y2 +1, which
is 1
u.
4
```

## PDF page 5

```text
2. Multiply by the derivative of the inner function with respect to x, which is
∂(x2+y2+1)
∂x
= 2x.
Putting it together, the partial derivative with respect to x is
∂f(x, y)
∂x
=
1
x2 + y2 + 1 · (2x) =
2x
x2 + y2 + 1.
Similarly, the partial derivative with respect to y is
∂f(x, y)
∂y
=
2y
x2 + y2 + 1.
(b) To find ∂f(x,y)
∂x
, we treat y as a constant, and use the chain rule:
1. Take the derivative of the outer function, √u, where u ≡xy + y3, which is
1
2√u.
2. Multiply by the derivative of the inner function with respect to x, which is
∂(xy+y3)
∂x
= y.
Putting it together, the partial derivative with respect to x is
∂f(x, y)
∂x
=
1
2
p
xy + y3 · (y) =
y
2
p
xy + y3.
Similarly, the partial derivative with respect to y is
∂f(x, y)
∂y
=
x + 3y2
2
p
xy + y3.
5
```
