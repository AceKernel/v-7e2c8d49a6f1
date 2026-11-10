# Tutorial 7 solutions: automatic text transcript

Original: [Tutorial 7 solutions PDF](tutorial-07-solutions.pdf). Topic: Complete supplied questions and official solutions.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050
S2 2026
Tutorial 7 Solution
Problem 1
Show that if g : R2 →R is a convex function and b ∈R then S = {(x, y) ∈R2 :
g(x, y) ≤b} is a convex set.
Solution: We have to show that if (x, y) ∈S, (x′, y′) ∈S and λ ∈[0, 1], then λ(x, y) + (1 −
λ)(x′, y′) ∈S. So let (x, y) ∈S, (x′, y′) ∈S and λ ∈[0, 1].
• (x, y) ∈S implies g(x, y) ≤b and thus
λg(x, y) ≤λb
(1)
• (x′, y′) ∈S implies g(x′, y′) ≤b and thus
(1 −λ)g(x′, y′) ≤(1 −λ)b
(2)
Thus
g(λ(x, y) + (1 −λ)(x′, y′)) ≤λg(x, y) + (1 −λ)g(x′, y′)
≤λb + (1 −λ)b = b,
where the first inequality follows from the convexity of g and the second inequality from
(1) and (2). But g(λ(x, y) + (1 −λ)(x′, y′)) ≤b means that λ(x, y) + (1 −λ)(x′, y′) ∈S.
This is what we wanted to show. Thus S is convex.
Note. S = {(x, y) ∈R2 : g(x, y) ≤b} is called the lower contour set of g for level b.
Similarly, S′ = {(x, y) ∈R2 : h(x, y) ≥a}, which is called the upper contour set of h for
level a. If h : R2 →R is a concave function and a ∈R then S′ is a convex set for every
a ∈R.
Problem 2
Suppose f : R2 →R can be written as
f(x, y) = g(x) + h(y),
where both g and h are convex functions of one variable. Show that f is also convex.
Solution: To show that f is convex, take any (x′, y′), (x′′, y′′) ∈R2 and λ ∈[0, 1]. Now
f(λ(x′, y′) + (1 −λ)(x′′, y′′)) = f(λx′ + (1 −λ)x′′, λy′ + (1 −λ)y′′)
= g(λx′ + (1 −λ)x′′) + h(λy′ + (1 −λ)y′′).
Because both g and h are convex,
g(λx′ + (1 −λ)x′′) ≤λg(x′) + (1 −λ)g(x′′),
1
```

## PDF page 2

```text
ECON 2050
S2 2026
and
h(λy′ + (1 −λ)y′′) ≤λh(y′) + (1 −λ)h(y′′).
Thus,
f(λ(x′, y′) + (1 −λ)(x′′, y′′)) = g(λx′ + (1 −λ)x′′) + h(λy′ + (1 −λ)y′′)
≤λg(x′) + (1 −λ)g(x′′) + λh(y′) + (1 −λ)h(y′′)
= λ[g(x′) + h(y′)] + (1 −λ)[g(x′′) + h(y′′)]
= λf(x′, y′) + (1 −λ)f(x′′, y′′)
By definition, f(x, y) is convex.
Problem 3
Show that the following sets are convex.
1. S = {(x, y) ∈R2 : y ≥x, x2 + y2 ≤4}
2. T = {(x, y) ∈R2 : y ≥x2, y ≤4}
Solution:
1. We observe that
• S1 = {(x, y) ∈R2 : y ≥x} is convex because S1 = epi(f1), where f1 : R →R
is given by f1(x) = x is a convex function (because it’s linear, and hence affine;
affine functions are both convex and concave).
(Alternatively, one may note that S1 = {(x, y) ∈R2 : x −y ≤0}. One can
use the result we proved in Problem 2 to show that fa(x, y) = x −y is a convex
function (let g(x) = x and h(y) = −y) and then apply the result we proved in
Problem 1.)
• S2 = {(x, y) ∈R2 : x2 + y2 ≤4} is convex by the result in Problem 1 because
we proved in lecture 7 that the function f2(x, y) = x2 + y2 is convex.
Thus, since S = S1∩S2 and since the intersection of convex sets is convex, S is convex.
Graphically,
2
```

## PDF page 3

```text
ECON 2050
S2 2026
2. We observe that
• T1 = {(x, y) ∈R2 : y ≥x2} is convex because T1 = epi(g1), where g1(x) = x2
is a convex function (one can prove it by taking second derivative to get g′′
1(x) =
2 > 0, or prove it using definition as in Problem 5).
(Alternatively, one may note that T1 = {(x, y) ∈R2 : x2 −y ≤0}. One can
use the result we proved in Problem 2 to show that ga(x, y) = x2 −y is a convex
function (let g(x) = x2 and h(y) = −y), and then apply the result in Problem 1.)
• T2 = {(x, y) ∈R2 : y ≤4} is convex by Problem 1 because g2(x, y) = y is a
convex function by the result we proved in Problem 2.
Thus, since T = T1∩T2 and since the intersection of convex sets is convex, T is convex.
Graphically,
Problem 4
Analyze whether the following functions are concave or convex.
1. f1(x, y) = 4x2 + e2y2.
2. f2(x, y) = ln(3x + 2y).
Solution:
1. Observe that f1(x, y) = g1(x) + h1(y), where g1(x) = 4x2, and h1(y) = e2y2. Now
g1(x) is convex, and h1(y) = m ◦n, where m(u) = eu is increasing and convex, and
n(y) = 2y2 is convex. Thus, both g1 and h1 are convex; by the result we proved in
Problem 2, f1(x, y) is also convex.
2. f2(x, y) = ln(3x + 2y) is concave because f2 = h2 ◦g2, where h2(u) = ln u is an
increasing concave function, and g2(x, y) = 3x + 2y is linear and hence concave.
Problem 5
Prove from the definition of a strictly convex function and without using any theorem
about convex functions that f(x) = x2 is strictly convex.
3
```

## PDF page 4

```text
ECON 2050
S2 2026
Solution: f is strictly convex if for all x′, x′′ ∈R such that x′ ̸= x′′, and all λ ∈(0, 1),
f(λx′ + (1 −λ)x′′) < λf(x′) + (1 −λ)f(x′′).
So let x′, x′′ ∈R be such that x′ ̸= x′′, and λ ∈(0, 1). Then
f(λx′ + (1 −λ)x′′) = (λx′ + (1 −λ)x′′)2 = λ2(x′)2 + 2λ(1 −λ)x′x′′ + (1 −λ)2(x′′)2
and
λf(x′) + (1 −λ)f(x′′) = λ(x′)2 + (1 −λ)(x′′)2.
Now observe that
λf(x′) + (1 −λ)f(x′′) −f(λx′ + (1 −λ)x′′)
= λ(x′)2 + (1 −λ)(x′′)2 −

λ2(x′)2 + 2λ(1 −λ)x′x′′ + (1 −λ)2(x′′)2
= (λ −λ2)(x′)2 −2λ(1 −λ)x′x′′ +

1 −λ −(1 −λ)2
(x′′)2
= λ(1 −λ)(x′)2 −2λ(1 −λ)x′x′′ + (1 −λ)[1 −(1 −λ)](x′′)2
= λ(1 −λ)

(x′)2 −2x′x′′ + (x′′)2
= λ(1 −λ)(x′ −x′′)2 > 0
where the strict inequality holds since x′ ̸= x′′ and λ ∈(0, 1). Hence f(λx′ + (1 −λ)x′′) <
λf(x′) + (1 −λ)f(x′′) and f is strictly convex.
Problem 6 (Extra Practice Problem)
Apply the result from Problem 1 and the properties of a convex set to demonstrate that
the following sets are convex.
1. S = {(x, y) ∈R2 : y ≥x2, x2 + y2 ≤4, x ≥0, y ≥0}
2. T = {(x, y) ∈R2 : x2 + y2 ≤25, x + y ≥5, y ≥2, x ≥0}
Solution: (Sketch only)
1. S is convex, as it is the intersection of the following sets, all of which are convex:
• S1 = {(x, y) ∈R2 : y ≥x2} (we showed in Problem 3 that it is convex),
• S2 = {(x, y) ∈R2 : y2 + x2 ≤4} (we showed in Problem 3 that it is convex),
• S3 = {(x, y) ∈R2 : −x ≤0} (convex by Problem 1 because f3(x, y) = −x is
affine and thus convex)
• S4 = {(x, y) ∈R2 : −y ≤0} (convex by Problem 1 because f4(x, y) = −y is
affine and thus convex)
Graphically:
4
```

## PDF page 5

```text
ECON 2050
S2 2026
2. T is convex, as it is the intersection of the following sets, all of which are convex:
• T1 = {(x, y) ∈R2 : y2 + x2 ≤25} (convex by Problem 1 because g1(x, y) =
x2 + y2 is convex, as we proved in lecture 7),
• T2 = {(x, y) ∈R2 : y ≥5 −x} (convex because T2 = epi(g2), where g2(x) =
5 −x is affine and thus convex),
• T3 = {(x, y) ∈R2 : −x ≤0} (convex by Problem 1 because f3(x, y) = −x is
affine and thus convex)
• T4 = {(x, y) ∈R2 : −y ≤−2} (convex by Problem 1 because f4(x, y) = −y is
affine and thus convex)
Graphically:
5
```
