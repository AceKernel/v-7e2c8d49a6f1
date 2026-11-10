# Logic: automatic text transcript

Original: [Logic PDF](logic.pdf). Topic: Logic and proof methods.

> Search aid only, not a verified LaTeX transcription. Fractions, exponents, matrices and figures may extract incorrectly. Check the original PDF and checked course guide.

## PDF page 1

```text
ECON 2050
Two-Valued Logic: A Very Brief Review
Every sentence expressing a proposition is either true (t) or false (f). Formally, such
sentences are all we deal with in ECON2050. For example: “Ann’s demand for coffee is
3 cups per week” or “The market price for a mufﬁn is $1.50” or “3 > 2” or “10+ 5 = 2.”
New propositions can be constructed from existing propositions A, B, C, ... through
logical operators:
Operator
New Proposition
not
¬
¬A
and
∧
A ∧B
or
∨
A ∨B
implies
⇒
A ⇒B (A implies B; if A then B; from A follows B; ...)
if and only if
⇔
A ⇔B (A is equivalent to B; A if and only if B)
The value of the new propositions is deﬁned as follows:
A
¬A
t
f
f
t
A
B
A ∧B
t
t
t
t
f
f
f
t
f
f
f
f
A
B
A ∨B
t
t
t
t
f
t
f
t
t
f
f
f
A
B
A ⇒B
t
t
t
t
f
f
f
t
t
f
f
t
A
B
A ⇔B
t
t
t
t
f
f
f
t
f
f
f
t
1
```

## PDF page 2

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

## PDF page 3

```text
and also that
¬(∃x ∈X : P(x))
if and only if
∀x ∈X : ¬P(x).
Example: Let X = {Ann, Bob, Charlie}. Ann is 169cm tall, Bob 187cm and Charlie
175cm. An intelligence test determines that Ann’s IQ is 137, Bob’s 128 and Charlie’s
141. (For a moment, the test administrator gets scared and thinks that she mistakenly
made the test too easy. But she calms down once she learns that Ann, Bob and Charlie just
completed ECON2050 at UQ.) Let P(x) = “x has an IQ of less than 140” and Q(x) =
“x is taller than 195cm.” Then ¬(∀x ∈X : P(x)) is true because ¬P(Charlie) is true.
Moreover, ¬(∃x ∈X : Q(x)) is true because (¬Q(Ann))∧(¬Q(Bob))∧(¬Q(Charlie))
is true.
In class we will sometimes have to prove that statements of the form ∀x ∈X : P(x)
are I) true, or, in other cases, that they are II) false.
II) is usually quite simple, thanks to (1): ∀x ∈X : P(x) is false if and only if
∃x ∈X : ¬P(x). Therefore, it is enough if we can ﬁnd one x ∈X for which P(x) is
false.
Example: Let X ≡{x ∈R : x > 0} and let’s prove that ∀x ∈X : x2 > x is
false. By (1), this is the case if and only if ∃x ∈X : ¬(x2 > x), that is, if and only if
∃x ∈X : x2 ≤x. And the latter statement is true as for x = 0.5, 0.25 = x2 ≤x = 0.5.
Done. We disproved ∀x > 0 : x2 > x by ﬁnding one example for which x2 > x is false.
I) is a bit more tricky. If we want to show that ∀x ∈X : P(x) is true, ﬁnding one
example for which P(x) is true is not enough.1 We need to show that P(x) is true for all
x ∈X. We usually are able to do this by arguing in the abstract.
Example: Let’s prove that ∀x ∈(2, ∞) : x2 > x. To do this, let x be any number strictly
greater than 2 (we won’t specify which, so that our argument is true for all numbers > 2).
From elementary math, we know that x2 > x is true if and only if x2
x > x
x is true. But the
latter is true if and only if x > 1. Since x > 1 is satisﬁed by every x > 2, we are done.
Home Exercise: Let X = {1, 2, 3} and N = {1, 2, 3, 4, ...}. Prove that the proposition
∀x ∈X∃y ∈X : y > x is false, while the proposition ∀x ∈N∃y ∈N : y > x is true.
Proof by Contradiction.
We often will need to demonstrate that for some propositions
A and B, the proposition A ⇒B has the value “true.” Recall that if A is false, then
A ⇒B is true regardless of the B’s value. Hence we can effectively focus on the case
that A is true and then argue that given this assumption, B must also be true.
1Unless X has only one element, but that is not a very interesting case...
3
```

## PDF page 4

```text
One technique that is often useful to prove that A ⇒B is true is called “proof by
contradiction.” Let C be a proposition that is false.2 The third and last columns of the
following truth-table
A
B
A ⇒B
¬B
A ∧¬B
C
(A ∧¬B) ⇒C
t
t
t
f
f
f
t
t
f
f
t
t
f
f
f
t
t
f
f
f
t
f
f
t
t
f
f
t
then show that
[A ⇒B] ⇔[(A ∧¬B) ⇒C].
Therefore, in order to prove that A ⇒B is true, we can show that for some false propo-
sition C, (A ∧¬B) ⇒C is true.
Example: Let us prove by contradiction that a sequence can have at most one limit (see
slides Lecture 1 p.20 and SB Thm 12.1). That is, let A = “(xn)n∈N is a sequence” and
B = “(xn)n∈N has at most one limit”. Suppose that
A ∧¬B = “(xn)n∈N is a sequence that has at least two limits.”
is true (remember that if A ∧¬B is false, then for every proposition C, (A ∧¬B) ⇒C
is true, and so we only need to worry about whether (A ∧¬B) ⇒C is true if (A ∧¬B)
is true). Let x∗and y∗be two distinct limits of (xn)n∈N. Then
ε ≡∥x∗−y∗∥
2
> 0.
Since x∗is a limit of (xn)n∈N, there exists a Nx∗∈N such that for all n ≥Nx∗,
∥xn −x∗∥< ε.
(2)
Similarly, since y∗is a limit of (xn)n∈N, there exists a Ny∗∈N such that for all n ≥
Ny∗,
∥xn −y∗∥< ε.
(3)
Let ¯n ≥max{Nx∗, Ny∗}. By (2) and (3),
∥x¯n −x∗∥< ε
∧
∥x¯n −y∗∥< ε.
Therefore, by the triangle inequality (see Slides 1, p. 21 and SB Thm 10.5),
∥x∗−y∗∥≤∥x∗−x¯n∥+∥x¯n −y∗∥= ∥x¯n −x∗∥+∥x¯n −y∗∥< ε+ε = ∥x∗−y∗∥.
Let C = “∥x∗−y∗∥< ∥x∗−y∗∥.” We showed that if (A ∧¬B) is true, then C is
true, as well. Since C is false, this completes our proof by contradiction. The following
ﬁgure, while not part of our proof, illustrates the intuition behind our argument in the
one-dimensional case.
2Note that for every proposition D, the proposition D ∧¬D is false (Exercise!). Hence we can obtain a
C that is false by taking an arbitrary proposition D and letting C = (D ∧¬D).
4
```

## PDF page 5

```text
R
N
x∗
y∗
x∗−ε = y∗+ ε
ε
ε
Nx∗
Ny∗
b
b
¯n
x¯n by (2)
x¯n by (3)
|x¯n −x∗|
|x¯n −y∗|
|x∗−y∗|
5
```
