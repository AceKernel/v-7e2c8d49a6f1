# Logic: Contradiction and contrapositive

PDF page 4 of 5.

[Page map](map-logic.md) | [Original PDF page](logic.pdf#page=4) | [Previous](page-logic-03.md) | [Next](page-logic-05.md)

Topics: notation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
