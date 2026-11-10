# Logic: Implication and quantifiers

PDF page 2 of 5.

[Page map](map-logic.md) | [Original PDF page](logic.pdf#page=2) | [Previous](page-logic-01.md) | [Next](page-logic-03.md)

Topics: notation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Note in particular the part of penultimate truth table highlighted in bold face: if A is
false, then A ⇒B is true.
Example: If A = “0 ≤2,” B = “3 = 3” and C = “10 < 7” then ¬A (that is, “0 > 2”),
¬B, A ∧C, A ⇔C and B ⇔C are all
false
, while ¬C, A ∨B, A ∧B, A ∨C and
A ⇔B are all
true
.
Example: If A =“Brisbane is the state capital of Tasmania” and B = “ECON2050 is
held at the UQ Gatton campus” then A ⇒B is true! Of course, we don’t meet for class
on the Gatton campus, but since A is false, the proposition A ⇒B is automatically true!
For the same reason, “If 1 > 2 then 3 + 3 = 7,” “If 1 > 2 then 3 + 3 = 6”, “If UQ is
located in Singapore, then the number of students enrolled in ECON2050 this semester
equals 2,137” and “If UQ is located in Singapore, then the number of students enrolled
in ECON2050 this semester does not equal 2,137” are all true.
Example: If A = “0 ≤2,” B = “3 = 3” and C = “5 + 2 = 9” then A ⇒B, B ⇒A,
C ⇒A and C ⇒B are all true, while A ⇒C and B ⇒C are both false.
Quantiﬁers.
We will also use the “universal quantiﬁer” ∀and the “existential quan-
tiﬁer” ∃to construct propositions. Intuitively, if X = {x1, x2, x3, . . .} is a set and a
proposition P(x) “depends on” the variable x ∈X, then
• ∀x ∈X : P(x) (“for all x in X, P(x),” or “P(x) is true for all x in X”) is a
proposition that is true if and only if P(x1) ∧P(x2) ∧P(x3) ∧. . . is true.
• ∃x ∈X : P(x) (“there exists a x in X such that P(x) is true,” or “there is a x ∈X
such that P(x)”) is a proposition that is true if and only if P(x1)∨P(x2)∨P(x3)∨
. . . is true.
Examples:
• The proposition ∀x ∈R : x + 1 > x is
true
.
• Let X = {Ann, Bob}. Ann likes cashews more than walnuts, and pecans more
than macadamia nuts. Bob likes cashews more than walnuts, and macadamia nuts
more than pecans. The proposition
– “∀x ∈X: x likes cashews more than walnuts” is
true
– “∃x ∈X: x likes cashews more than walnuts” is
true
– “∀x ∈X: x likes pecans more than macadamia nuts” is
false
– “∃x ∈X: x likes pecans more than macadamia nuts” is
true
Note that
¬(∀x ∈X : P(x))
if and only if
∃x ∈X : ¬P(x),
(1)
2
```
