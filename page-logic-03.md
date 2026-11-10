# Logic: Negating quantified statements

PDF page 3 of 5.

[Page map](map-logic.md) | [Original PDF page](logic.pdf#page=3) | [Previous](page-logic-02.md) | [Next](page-logic-04.md)

Topics: notation.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

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
