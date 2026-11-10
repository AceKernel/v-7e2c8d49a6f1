# Tutorial 9 solutions: P5: Factory operating-cost minimisation and its dual

PDF page 6 of 6.

[Page map](map-tutorial-09-solutions.md) | [Original PDF page](tutorial-09-solutions.pdf#page=6) | [Previous](page-tutorial-09-solutions-05.md)

Topics: duality.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
ECON 2050
S2 2026
An electronics firm that produces phones and tablets has two factories that jointly pro-
duce the two goods in the following quantities per hour:
Factory 1
Factory 2
Phones
10
20
Tablets
25
25
The firm receives an order for 300 phones and 500 tablets. The costs of operating the two
factories are $10000 and $8000 per hour, respectively.
(a) Formulate the linear programming problem of minimizing the total cost of meeting this
order.
(b) Write down the equivalent maximization problem, and then find its dual.
Solution:
(a) Let 𝑥1 and 𝑥2 denote the number of hours for which the two factories operate to produce
the order. Then the above table tells us that a total of 10𝑥1 + 20𝑥2 phones is produced,
as well as 25𝑥1 + 25𝑥2 tablets. Because 300 phones and 500 tablets are required, the pair
(𝑥1, 𝑥2) must satisfy
10𝑥1 + 20𝑥2 ≥300
25𝑥1 + 25𝑥2 ≥500
In addition, of course, 𝑥1 ≥0 and 𝑥2 ≥0. The total cost of operating the two factories for
𝑥1 and 𝑥2 hours, respectively, is 10000𝑥1 + 8000𝑥2. The problem is, therefore,
min 10000𝑥1 + 8000𝑥2
s.t.
{
10𝑥1 + 20𝑥2 ≥300
25𝑥1 + 25𝑥2 ≥500 and 𝑥1 ≥0, 𝑥2 ≥0
(b) The linear programming problem above is equivalent to (also changed ≥to ≤in the
constraints)
max −10000𝑥1 −8000𝑥2
s.t.
{
−10𝑥1 −20𝑥2 ≤−300
−25𝑥1 −25𝑥2 ≤−500 and 𝑥1 ≥0, 𝑥2 ≥0
Its dual is
min −300𝑦1 + −500𝑦2
s.t.
{
−10𝑦1 −25𝑦2 ≥−10000
−20𝑦1 −25𝑦2 ≥−8000
and 𝑦1 ≥0, 𝑦2 ≥0
6
```
