# Lecture 3: Chain-rule exercises

PDF page 8 of 31; printed slide 8.

[Page map](map-lecture-03.md) | [Original PDF page](lecture-03.pdf#page=8) | [Previous](page-lecture-03-07.md) | [Next](page-lecture-03-09.md)

Topics: chain-hessian.

> Unverified automatic extraction; fractions, exponents, matrices, symbols and figures may be corrupted. Check the original PDF. Source text is retained, not corrected or converted into verified LaTeX.

```text
Exercises:
Calculate the derivative of ˜h(x) = ln(x2 + 4).
We first observe that ˜h(x) = (˜g ◦˜f )(x), where ˜g(y) ≡ln y, and ˜f (x) ≡x2 + 4.
By the chain rule,
˜h′(x) = ˜g′(˜f (x))˜f ′(x) = [ln(˜f (x))]′ ˜f ′(x) =
1
˜f (x)
˜f ′(x) =
2x
x2 + 4.
Calculate the derivative of ¯h(x) = e1/x.
We first observe that ¯h(x) = (¯g ◦¯f )(x), where ¯g(y) ≡ey, and ¯f (x) ≡1/x.
By the chain rule,
¯h′(x) = ¯g′(¯f (x))¯f ′(x) =
[︂
e
˜f (x)]︂′ ˜f ′(x) = e
˜f (x) ˜f ′(x) = −e
1
x
x2 .
ECON 2050 – Basic Real Analysis III
8 / 31
```
